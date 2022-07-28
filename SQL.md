# 1、foreach

```xml
<select id="queryStatisticaSafe" parameterType="java.util.Map" resultType="java.util.Map">
        SELECT
        (select ra.name from rm_area ra where ra.id = t1.region_id),
        count(1)
        FROM
        im_sg_safeguard t1,ir_sg_safeguard_entity t2
        WHERE
        t1.id = t2.safeguard_id
        <if test="safeId!= null and safeId !='' and statistical==1">
            AND t1.id  =  #{safeId,jdbcType=NUMERIC}
        </if>
        <if test="regionIds != null">
            AND t1.region_id IN
            <foreach collection="regionIds" item="item" separator="," open="(" close=")">
                #{item}
            </foreach>
        </if>
        <if test="specIds != null and statistical==2">
            AND t2.entity_spec_id IN
            <foreach collection="specIds" item="item" separator="," open="(" close=")">
                #{item}
            </foreach>
        </if>
        <if test="specId!= null and specId !='' and statistical==3">
            AND t2.entity_spec_id  =  #{specId,jdbcType=NUMERIC}
        </if>
        group by t1.region_id
    </select>
```

# 2、if 、when、choose 、otherwise

```xml
 <select id="listQueryQrcodeManager" parameterType="java.util.Map" resultType="java.util.Map">
        SELECT
        <if test="tableName != 'RM_PRODUCT'">
            t1.name,
            t1.region_id,
            t1.DATA_SOURCE_ID,
            (select name from rm_area ra where ra.id = t1.region_id)region_id_name,
            (select zone_number from rm_area ra where ra.id = t1.region_id)zone_number,
        </if>
        <if test="tableName != 'RM_PRODUCT'  and tableName != 'CM_LINK'">
            t1.ADDRESS_DESC,
            t1.LIFE_STATE_ID,
        </if>
        <if test="tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
            <if test="tableName != 'CM_WARE'">
                t1.LONGITUDE,
                t1.LATITUDE,
            </if>
            (select name from DM_MODEL dm where dm.id = t1.MODEL_ID)model_code,
            (select name from DM_MANUFACTOR dmr where dmr.id = t1.MANUFACTOR_ID)manufactor_code,
            (select zone_number from rm_area ra where ra.id = t1.region_id)zoneNumber,
               <choose>
                   <when test="tableName == 'CM_FACILITY'">
                       t1.name room_name,
                   </when>
                   <otherwise>
                       (select name from CM_FACILITY tp where tp.id = t1.FACILITY_ID) room_name,
                   </otherwise>
               </choose>

            (select name from RM_AREA tp where tp.id = t1.tml_id) site_name,
            (select
               (case rp.spec_id
                  when 2930100001 then (select name from RE_PROJECT_MSS rs where rs.project_id  = rp.id)
                  when 2930100002 then (select name from RE_PROJECT_RESOURCE rr where   rr.project_id  = rp.id)
                end)
              from rm_project rp,rr_project_entity rre
              where rp.id = rre.project_id and t1.id = rre.entity_id) project_name,
            (select ra.name from RR_AREA_ENTITY rra,rm_area ra
            where rra.entity_id  =t1.id
            and rra.area_id  = ra.id and t1.spec_id  = rra.entity_spec_id
            and rra.area_spec_id = ra.spec_id and rra.spec_id = 1025222110000) site_direction_name,
        </if>
        <if test="tableName == 'CM_LINK'">
            t1.DATA_SOURCE_ID,
            t1.region_id,
            (select name from rm_area ra where ra.id = t1.region_id)region_id_name,
<!--            (select-->
<!--            (case rp.spec_id-->
<!--            when 2930100001 then (select name from RE_PROJECT_MSS rs where rs.project_id  = rp.id)-->
<!--            when 2930100002 then (select name from RE_PROJECT_RESOURCE rr where   rr.project_id  = rp.id)-->
<!--            end)-->
<!--            from rm_project rp,rr_project_entity rre-->
<!--            where rp.id = rre.project_id and t1.id = rre.entity_id) project_name,-->
            t1.a_physic_device_id,
            t1.z_physic_device_id,
            (select code from cm_device cd  WHERE cd.id=t1.a_physic_device_id) a_code,
            (select name from cm_device cd  WHERE cd.id=t1.a_physic_device_id) a_name,
            (select address_desc from cm_device cd  WHERE cd.id=t1.a_physic_device_id) a_address_desc,
            (select latitude from cm_device cd  WHERE cd.id=t1.a_physic_device_id) a_latitude,
            (select longitude from cm_device cd  WHERE cd.id=t1.a_physic_device_id) a_longitude,
            (select code from cm_device cd  WHERE cd.id=t1.z_physic_device_id) z_code,
            (select name from cm_device cd  WHERE cd.id=t1.z_physic_device_id) z_name,
            (select address_desc from cm_device cd  WHERE cd.id=t1.z_physic_device_id) z_address_desc,
            (select latitude from cm_device cd  WHERE cd.id=t1.z_physic_device_id) z_latitude,
            (select longitude from cm_device cd  WHERE cd.id=t1.z_physic_device_id) z_longitude,
        </if>
        <if test="tableName == 'CM_CABLE'">
            t1.a_device_id,
            t1.z_device_id,
            (select code from cm_device cd  WHERE cd.id=t1.a_device_id) a_code,
            (select name from cm_device cd  WHERE cd.id=t1.a_device_id) a_name,
            (select address_desc from cm_device cd  WHERE cd.id=t1.a_device_id) a_address_desc,
            (select latitude from cm_device cd  WHERE cd.id=t1.a_device_id) a_latitude,
            (select longitude from cm_device cd  WHERE cd.id=t1.a_device_id) a_longitude,
            (select code from cm_device cd  WHERE cd.id=t1.z_device_id) z_code,
            (select name from cm_device cd  WHERE cd.id=t1.z_device_id) z_name,
            (select address_desc from cm_device cd  WHERE cd.id=t1.z_device_id) z_address_desc,
            (select latitude from cm_device cd  WHERE cd.id=t1.z_device_id) z_latitude,
            (select longitude from cm_device cd  WHERE cd.id=t1.z_device_id) z_longitude,
        </if>
        t1.code,
        t1.spec_id,
        t1.id,
        t2.qrcode,
        t2.id qrcodeId,
        t5.is_print
        FROM
        <if test="site != null and site !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
            RM_AREA t4,
        </if>
        <if test="room != null and room !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
            CM_FACILITY t3,
        </if>
        im_label_qrcode t2,
        <if test="specId != 1121000002">
          im_label_point_CODE_LOG t5,
        </if>
        <if test="specId == 1121000002">
          im_label_line_CODE_LOG t5,
        </if>
        <if test="project != null and project !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE'">
            rr_project_entity t6,
        </if>
        <if test="siteDirection != null and siteDirection !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE'">
            RR_AREA_ENTITY t7,
        </if>
        ${tableName} t1
        <where>
            t1.spec_id = t2.entity_spec_id
            AND
            t1.id = t2.entity_id
            AND
            t1.spec_id = t5.entity_spec_id
            AND
            t1.id = t5.entity_id
            <if test="specId != null and specId!= ''">
                AND t1.spec_id = #{specId,jdbcType=NUMERIC}
            </if>
            <if test="regionId != null and regionId != '' and tableName != 'RM_PRODUCT'">
                AND t1.region_id IN
                (with recursive tree AS (
                select ar.id,ar.parent_id ,ar.name from RM_AREA ar where ar.id = #{regionId,jdbcType=NUMERIC}
                union all
                select ar.id,ar.parent_id ,ar.name from RM_AREA ar inner join tree on ar.parent_id = tree.id and ar.is_valid in(1001,100383)
                ) select id from tree)
                <!--<foreach collection="regionIds" item="item" separator="," open="(" close=")">
                    #{item}
                </foreach>-->
            </if>
            <if test="resourceState != null and resourceState!= ''">
                AND t1.LIFE_STATE_ID = #{resourceState,jdbcType=NUMERIC}
            </if>
            <if test="name != null and name!= '' and tableName != 'RM_PRODUCT'">
                AND t1.name LIKE concat('%',#{name,jdbcType=VARCHAR},'%')
            </if>
            <if test="addressDesc != null and addressDesc!= '' and tableName != 'RM_PRODUCT'">
                AND t1.address_desc LIKE concat('%',#{addressDesc,jdbcType=VARCHAR},'%')
            </if>
            <if test="code != null and code!= ''">
                AND t1.code LIKE concat('%',#{code,jdbcType=VARCHAR},'%')
            </if>
            <if test="startTime!=null and endTime!=null">
                AND t1.create_date <![CDATA[ >= ]]> #{startTime,jdbcType=TIMESTAMP}
                AND t1.create_date <![CDATA[ <= ]]> #{endTime,jdbcType=TIMESTAMP}
            </if>
            <if test="site != null and site !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
                AND t4.id = #{site,jdbcType=NUMERIC}
                AND t4.id = t1.tml_id
            </if>
            <if test="room != null and room !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
                AND t3.id = #{room,jdbcType=NUMERIC}
                AND t3.id = t1.FACILITY_ID
            </if>
            <if test="qrIdentification == 1">
                AND t5.is_print = 1
            </if>
            <if test="qrIdentification == 2">
                AND t5.is_print = 0
            </if>
            <if test="qrIdentification == 3">
                AND t5.is_paste = 1
            </if>
            <if test="qrIdentification == 4">
                AND t5.is_paste = 0
            </if>
            <if test="project != null and project !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE'">
                AND t6.project_id = #{project,jdbcType=NUMERIC}
                AND t6.entity_id = t1.id
            </if>
            <if test="siteDirection != null and siteDirection !='' and tableName != 'RM_PRODUCT' and tableName != 'CM_CABLE' and tableName != 'CM_LINK'">
                AND t7.area_id = #{siteDirection,jdbcType=NUMERIC}
                AND t7.entity_id = t1.id
            </if>
        </where>
    </select>
```

# 3、动态update的SQL

```
<update id="updateOne"  parameterType="com.inspur.search.data.EntityRelation">
 UPDATE ENTITY_RELATION
 <trim prefix="set" suffixOverrides=",">
  <if test="srcId!=null">SRC_ID=#{srcId},</if>
  <if test="srcType!=null">SRC_TYPE=#{srcType},</if>
  <if test="destId!=null">DEST_ID=#{destId},</if>
  <if test="destType!=null">DEST_TYPE=#{destType},</if>
  <if test="relType!=null">REL_TYPE=#{relType},</if>
  <if test="status!=null">STATUS=#{status},</if>
  <if test="snId!=null">SN_ID=#{snId},</if>
 </trim>
 WHERE id=#{id}
</update>
```

# 4、日期更新的时候应该注意

```xml
<if test="project != null and project !=''></if>上面这个是错误的
<if test="project != null ></if>下面这个是对的
```

# 5、mapper.xml中的大于、小于、不等于需要转义

```xml
小于： &lt;
大于： &gt;
不等于： &lt;&gt;
大于等于： &gt;=
```

# 6、存储过程

```xml
    <select id="listQueryOcableDistbt" statementType="CALLABLE" resultMap="RM_OcableDistbt" >
        {call func_ocable_distribution(
                #{ocableId, mode=IN}
            )}
    </select>
    <select id="queryOcableStatis" statementType="CALLABLE" resultMap="RM_OcableStatis" >
        {call func_ocable_statistics(
                #{ocableId, mode=IN}
            )}
    </select>
在调用存储过程的方法中，我们需要把 statementType 设置为 CALLABLE，在使用 select 元素中调用存储过程时，由于存储过程方式不支持 MyBatis 的二级缓存（后面章节会介绍），为了避免缓存配置导致出错，我们直接将 select 元素的 useCache 属性设置为 false。

在存储过程中使用参数时，除了写上必要的属性名外，还必须指定参数的 mode（模式），可选值为 IN、OUT、INOUT 三种，入参使用 IN，出参使用 OUT，输入输出参数使用 INOUT。从上面代码可以轻易看出 IN 和 OUT 的两种模式的区别，那就是 OUT 模式的参数，必须指定 jdbcType。这是因为在 IN 模式下，MyBatis 提供了默认的 jdbcType，在 OUT 模式下没有提供，因此必须指定 jdbcType，另外在使用 Oracle 数据库时，如果入参存在 null 的情况，那么也必须指定 jdbcType。

除了上面提到的这几点外，headImg 还特别设置了 javaType。在 MyBatis 映射的 Java 类中我们都不推荐使用基本类型，但是数据库 BLOB 类型对应的 Java 类型我们通常都是写成 byte[] 字节数组，因为 byte[] 数组不会有默认值的问题，所以不会影响我们一般的使用。但是在不指定 javaType的情况下，MyBatis 默认使用 Byte 类型。由于我们使用的 byte 是基本类型，所以设置 javaType的时候，基本类型要使用带下划线方式的类型，在这里就是 byte[]，_byte 对应的是基本类型，byte 对应的是 Byte 类型，在使用 javaType 时一定要注意。
```

# 7、like concat()防止SQL注入

```xml
对于mysql 的 like 而言，一般都要用 like concat() 组合，可以防止sql注入         

  所以用未注释掉的呢种方式会比较好，不推荐直接用like的方式 。

            like concat('%/',#{datePath,jdbcType=VARCHAR},'/%')

            concat函数：
               第一个参数 ，就是'%'，其中%后边可以加上一些常量字符比如  / 。
               第二参数，基本上就是传递过来的参数 。
               第三个参数，是结尾的 '%'， %前边可以加一定的常量字符比如  / 。


 XXX  LIKE CONCAT('%', #xxx#, '%')
```

# 8、rank() over、dense_rank() over、row_number() over

```xml

```

![1649725715151](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\1649725715151.png)

![1649725730425](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\1649725730425.png)

```xml

```

![1649725756724](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\1649725756724.png)

# 9、SQL中的类型转换cast(：：) convert 

```xml
 select t2.id from gp_rscmap t2,im_gis_point t where entity_id = t2.rsc_id :: numeric
select * from gp_rscmap t2 where t.entity_id = cast(t2.rsc_id as numeric(24)
```

# 10、with recursive

```
ql中with xxxx as () 是对一个查询子句做别名，同时数据库会对该子句生成临时表；

with recursive 则是一个递归的查询子句，他会把查询出来的结果再次代入到查询子句中继续查询，如下面的语句
	with recursive t as (select id, parent_id
		from sm_menu
		where code = #{systemCode,jdbcType=VARCHAR}
		union all
		select k.id, k.parent_id
		from sm_menu k,
		t
		where t.id = k.parent_id)
```

# 11、trim prefix="(" suffix=")" suffixOverrides=","

```
  INSERT INTO gis_layer_control 
        <trim prefix="(" suffix=")" suffixOverrides=",">
        	<if test="controlId != null">
                control_id,
            </if>
        	<if test="layerId != null">
                layer_id,
            </if>
        	<if test="groupId != null">
                group_id,
            </if>
        	<if test="rscSpecId != null">
                rsc_spec_id,
            </if>
        	<if test="rscSpecName != null">
                rsc_spec_name,
            </if>
        	<if test="icon != null">
                icon,
            </if>
        	<if test="minScale != null">
                min_scale,
            </if>
        	<if test="maxScale != null">
                max_scale,
            </if>
        	<if test="isShow != null">
                is_show,
            </if>
        	<if test="description != null">
                description,
            </if>
        </trim>
        <trim prefix="values (" suffix=")" suffixOverrides=",">
        	<if test="controlId != null">
                #{controlId,jdbcType=INTEGER},
            </if>
        	<if test="layerId != null">
                #{layerId,jdbcType=INTEGER},
            </if>
        	<if test="groupId != null">
                #{groupId,jdbcType=INTEGER},
            </if>
        	<if test="rscSpecId != null">
                #{rscSpecId,jdbcType=NUMERIC},
            </if>
        	<if test="rscSpecName != null">
                #{rscSpecName,jdbcType=VARCHAR},
            </if>
        	<if test="icon != null">
                #{icon,jdbcType=VARCHAR},
            </if>
        	<if test="minScale != null">
                #{minScale,jdbcType=INTEGER},
            </if>
        	<if test="maxScale != null">
                #{maxScale,jdbcType=INTEGER},
            </if>
        	<if test="isShow != null">
                #{isShow,jdbcType=SMALLINT},
            </if>
        	<if test="description != null">
                #{description,jdbcType=VARCHAR},
            </if>
        </trim>
```

# 12、foreach collection

```
select ttt.* from
		(select t.code,tt.params_value,t.id from
		(select * from sm_menu where menu_type_id=83200023) t,
		sm_menu tt
		where t.parent_id = tt.id) ttt,sr_role_menu r
		where ttt.id = r.menu_id and r.role_id in
		<foreach collection="userRoles" open="("  close=")" separator="," item="item">
			#{item.id}
		</foreach>
```



# 13、


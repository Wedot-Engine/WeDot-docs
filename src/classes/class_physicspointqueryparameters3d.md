<!-- ⚠ 请勿编辑本文件 ⚠ -->
<!-- 本文档使用脚本从 WeDot 引擎源码仓库生成。 -->
<!-- 生成脚本：https://github.com/WeDot-Engine/WeDot/tree/4.3/doc/tools/make_md.py； -->
<!-- 原文件：https://github.com/WeDot-Engine/WeDot/tree/4.3/doc/classes/PhysicsPointQueryParameters3D.xml。 -->

<div id="_class_physicspointqueryparameters3d"></div>

# PhysicsPointQueryParameters3D

**继承：** [`RefCounted`](class_refcounted.md) **<** [`Object`](class_object.md)

Provides parameters for [`PhysicsDirectSpaceState3D.intersect_point`](#class_physicsdirectspacestate3d_method_intersect_point).

## 描述

By changing various properties of this object, such as the point position, you can configure the parameters for [`PhysicsDirectSpaceState3D.intersect_point`](#class_physicsdirectspacestate3d_method_intersect_point).

## 属性

| [`bool`](class_bool.md)                       | [`collide_with_areas`](#class_physicspointqueryparameters3d_property_collide_with_areas)   | ``false``            |
| [`bool`](class_bool.md)                       | [`collide_with_bodies`](#class_physicspointqueryparameters3d_property_collide_with_bodies) | ``true``             |
| [`int`](class_int.md)                         | [`collision_mask`](#class_physicspointqueryparameters3d_property_collision_mask)           | ``4294967295``       |
| [Array](class_array.md) [`RID`](class_rid.md) | [`exclude`](#class_physicspointqueryparameters3d_property_exclude)                         | ``[]``               |
| [`Vector3`](class_vector3.md)                 | [`position`](#class_physicspointqueryparameters3d_property_position)                       | ``Vector3(0, 0, 0)`` |

<!-- rst-class:: classref-section-separator -->

---

## 属性说明

<div id="_class_physicspointqueryparameters3d_property_collide_with_areas"></div>

[`bool`](class_bool.md) **collide_with_areas** = ``false`` <div id="class_physicspointqueryparameters3d_property_collide_with_areas"></div>

- `void` **set_collide_with_areas** ( value: [`bool`](class_bool.md) )
- [`bool`](class_bool.md) **is_collide_with_areas_enabled** ( )

If `true`, the query will take [`Area3D`](class_area3d.md) s into account.

<!-- rst-class:: classref-item-separator -->

---

<div id="_class_physicspointqueryparameters3d_property_collide_with_bodies"></div>

[`bool`](class_bool.md) **collide_with_bodies** = ``true`` <div id="class_physicspointqueryparameters3d_property_collide_with_bodies"></div>

- `void` **set_collide_with_bodies** ( value: [`bool`](class_bool.md) )
- [`bool`](class_bool.md) **is_collide_with_bodies_enabled** ( )

If `true`, the query will take [`PhysicsBody3D`](class_physicsbody3d.md) s into account.

<!-- rst-class:: classref-item-separator -->

---

<div id="_class_physicspointqueryparameters3d_property_collision_mask"></div>

[`int`](class_int.md) **collision_mask** = ``4294967295`` <div id="class_physicspointqueryparameters3d_property_collision_mask"></div>

- `void` **set_collision_mask** ( value: [`int`](class_int.md) )
- [`int`](class_int.md) **get_collision_mask** ( )

The physics layers the query will detect (as a bitmask). By default, all collision layers are detected. See [*Collision layers and masks*](../tutorials/physics/physics_introduction.md#collision-layers-and-masks) in the documentation for more information.

<!-- rst-class:: classref-item-separator -->

---

<div id="_class_physicspointqueryparameters3d_property_exclude"></div>

[Array](class_array.md) [`RID`](class_rid.md) **exclude** = ``[]`` <div id="class_physicspointqueryparameters3d_property_exclude"></div>

- `void` **set_exclude** ( value: [Array](class_array.md) [`RID`](class_rid.md) )
- [Array](class_array.md) [`RID`](class_rid.md) **get_exclude** ( )

The list of object [`RID`](class_rid.md) s that will be excluded from collisions. Use [`CollisionObject3D.get_rid`](#class_collisionobject3d_method_get_rid) to get the [`RID`](class_rid.md) associated with a [`CollisionObject3D`](class_collisionobject3d.md)-derived node.

 **Note:** The returned array is copied and any changes to it will not update the original property value. To update the value you need to modify the returned array, and then assign it to the property again.

<!-- rst-class:: classref-item-separator -->

---

<div id="_class_physicspointqueryparameters3d_property_position"></div>

[`Vector3`](class_vector3.md) **position** = ``Vector3(0, 0, 0)`` <div id="class_physicspointqueryparameters3d_property_position"></div>

- `void` **set_position** ( value: [`Vector3`](class_vector3.md) )
- [`Vector3`](class_vector3.md) **get_position** ( )

The position being queried for, in global coordinates.

[^virtual]: 本方法通常需要用户覆盖才能生效。
[^const]: 本方法无副作用，不会修改该实例的任何成员变量。
[^vararg]: 本方法除了能接受在此处描述的参数外，还能够继续接受任意数量的参数。
[^constructor]: 本方法用于构造某个类型。
[^static]: 调用本方法无需实例，可直接使用类名进行调用。
[^operator]: 本方法描述的是使用本类型作为左操作数的有效运算符。
[^bitfield]: 这个值是由下列位标志构成位掩码的整数。
[^void]: 无返回值。
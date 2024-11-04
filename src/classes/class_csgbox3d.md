<!-- ⚠ 请勿编辑本文件 ⚠ -->
<!-- 本文档使用脚本从 WeDot 引擎源码仓库生成。 -->
<!-- 生成脚本：https://github.com/WeDot-Engine/WeDot/tree/4.3/doc/tools/make_md.py； -->
<!-- 原文件：https://github.com/WeDot-Engine/WeDot/tree/4.3/modules/csg/doc_classes/CSGBox3D.xml。 -->

<div id="_class_csgbox3d"></div>

# CSGBox3D

**继承：** [`CSGPrimitive3D`](class_csgprimitive3d.md) **<** [`CSGShape3D`](class_csgshape3d.md) **<** [`GeometryInstance3D`](class_geometryinstance3d.md) **<** [`VisualInstance3D`](class_visualinstance3d.md) **<** [`Node3D`](class_node3d.md) **<** [`Node`](class_node.md) **<** [`Object`](class_object.md)

A CSG Box shape.

## 描述

This node allows you to create a box for use with the CSG system.

 **Note:** CSG nodes are intended to be used for level prototyping. Creating CSG nodes has a significant CPU cost compared to creating a [`MeshInstance3D`](class_meshinstance3d.md) with a [`PrimitiveMesh`](class_primitivemesh.md). Moving a CSG node within another CSG node also has a significant CPU cost, so it should be avoided during gameplay.

## 属性

| [`Material`](class_material.md) | [`material`](#class_csgbox3d_property_material) |                      |
| [`Vector3`](class_vector3.md)   | [`size`](#class_csgbox3d_property_size)         | ``Vector3(1, 1, 1)`` |

<!-- rst-class:: classref-section-separator -->

---

## 属性说明

<div id="_class_csgbox3d_property_material"></div>

[`Material`](class_material.md) **material** <div id="class_csgbox3d_property_material"></div>

- `void` **set_material** ( value: [`Material`](class_material.md) )
- [`Material`](class_material.md) **get_material** ( )

The material used to render the box.

<!-- rst-class:: classref-item-separator -->

---

<div id="_class_csgbox3d_property_size"></div>

[`Vector3`](class_vector3.md) **size** = ``Vector3(1, 1, 1)`` <div id="class_csgbox3d_property_size"></div>

- `void` **set_size** ( value: [`Vector3`](class_vector3.md) )
- [`Vector3`](class_vector3.md) **get_size** ( )

The box's width, height and depth.

[^virtual]: 本方法通常需要用户覆盖才能生效。
[^const]: 本方法无副作用，不会修改该实例的任何成员变量。
[^vararg]: 本方法除了能接受在此处描述的参数外，还能够继续接受任意数量的参数。
[^constructor]: 本方法用于构造某个类型。
[^static]: 调用本方法无需实例，可直接使用类名进行调用。
[^operator]: 本方法描述的是使用本类型作为左操作数的有效运算符。
[^bitfield]: 这个值是由下列位标志构成位掩码的整数。
[^void]: 无返回值。
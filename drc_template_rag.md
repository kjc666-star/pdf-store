# DRC模板-第二行语法结构RAG知识库
## 说明
- 本知识库为DRC代码生成专用，每个模板名对应唯一的第二行SVRF指令语法结构
- LLM使用规则：根据输入的模板名，匹配对应语法结构，替换{变量}后输出最终指令




MinWidth: INT {layer1} < {value} ABUT < 90 SINGULAR REGION
MinWidth_Inside: INT {layer1} < {value} ABUT < 90 INSIDE {layer2} REGION
FixedWidth: INT {layer1} == {value} ABUT < 90 SINGULAR REGION
FixedWidth_Inside: INT {layer1} == {value} ABUT < 90 INSIDE {layer2} REGION
FixedWidth_Except: INT {layer1} == {value} ABUT < 90 EXCEPT {layer2} REGION
MinSpacing: EXT {layer1} {layer2} < {value} REGION
MinSpacing_Inside: EXT {layer1} {layer2} < {value} INSIDE {layer3} REGION
MinSpacing_Except: EXT {layer1} {layer2} < {value} EXCEPT {layer3} REGION
MinSpacing_InterLayer: EXT {layer1} {layer2} < {value} INTERLAYER REGION
MinSpacing_InterLayer_Inside: EXT {layer1} {layer2} < {value} INTERLAYER INSIDE {layer3} REGION
MinSpacing_InterLayer_Except: EXT {layer1} {layer2} < {value} INTERLAYER EXCEPT {layer3} REGION
MinSpacing_Conditional: EXT {layer1} {layer2} < {value} CONDITIONAL {condition} REGION
MinEnclosure: INT {layer1} {layer2} < {value} ENCLOSURE REGION
MinEnclosure_With_Tol: INT {layer1} {layer2} < {value} ENCLOSURE TOLERANCE {tol} REGION
MinEnclosure_Inside: INT {layer1} {layer2} < {value} ENCLOSURE INSIDE {layer3} REGION
MinEnclosure_Except: INT {layer1} {layer2} < {value} ENCLOSURE EXCEPT {layer3} REGION
L1InsideL2: INT {layer1} NOT {layer2} INSIDE REGION
L1InteractL2: INT {layer1} {layer2} INTERACT REGION
FixedLengthByOrthogonal: INT {layer1} == {value} ORTHOGONAL LENGTH REGION
MinDiameter: INT {layer1} < {value} ABUT < 90 SINGULAR REGION
MinDiameter_Except: INT {layer1} < {value} ABUT < 90 EXCEPT {layer2} REGION
MinDiameter_Inside: INT {layer1} < {value} ABUT < 90 INSIDE {layer2} REGION
Density_Global_Max: INT {layer1} > {value} DENSITY GLOBAL REGION
Density_Global_Min: INT {layer1} < {value} DENSITY GLOBAL REGION
Density_Window_Max: INT {layer1} > {value} DENSITY WINDOW {window} REGION
Density_Window_Min: INT {layer1} < {value} DENSITY WINDOW {window} REGION
Density_Region_Max: INT {layer1} > {value} DENSITY REGION {layer2} REGION
Density_Region_Min: INT {layer1} < {value} DENSITY REGION {layer2} REGION
FixedOffset_XY: INT {layer1} OFFSET {x_offset} {y_offset} REGION
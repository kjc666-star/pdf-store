DRC模板-第二行语法结构RAG知识库

本知识库为DRC代码生成专用，每个模板名对应唯一的第二行SVRF指令语法结构，结构为：模板名————语法结构（一一对应）
使用规则：依次根据模板名，匹配对应语法结构，生成对应结构函数



模板名                                                          语法结构
MinWidth  ———————————————————————————    INT {layer1} < {value} ABUT < 90 SINGULAR REGION
MinWidth_Inside—————————————————————————  INT {layer1} < {value} ABUT < 90 SINGULAR INSIDE {layer2} REGION
FixedWidth———————————————————————————   INT {layer1} = {value} ABUT < 90 SINGULAR REGION
FixedWidth_Inside————————————————————————    INT {layer1} = {value} ABUT < 90 SINGULAR INSIDE {layer2} REGION
FixedWidth_Except————————————————————————   INT {layer1} < {value} ABUT < 90 SINGULAR EXCEPT {layer2} REGION
MinSpacing———————————————————————————     EXT {layer1} < {value} ABUT < 90 SINGULAR REGION
MinSpacing_Inside————————————————————————      EXT {layer1} < {value} ABUT < 90 SINGULAR INSIDE {layer2} REGION
MinSpacing_Except————————————————————————    EXT {layer1} < {value} ABUT < 90 SINGULAR EXCEPT {layer2} REGION
MinSpacing_InterLayer———————————————————————   EXT {layer1} {layer2} < {value} ABUT < 90 SINGULAR REGION
MinSpacing_InterLayer_Inside————————————————————   EXT {layer1} {layer2} < {value} ABUT < 90 SINGULAR INSIDE {layer3} REGION
MinSpacing_InterLayer_Except———————————————————— EXT {layer1} {layer2} < {value} ABUT < 90 SINGULAR INSIDE {layer3} REGION
MinSpacing_Conditional—————————————————————EXT {layer1} < {value} IF DIAMETER {layer1} = {num1} ABUT < 90 SINGULAR REGION
MinEnclosure——————————————————————————ENC {layer1} {layer2} < {value} ABUT < 90 SINGULAR REGION
MinEnclosure_With_Tol——————————————————————ENC {layer1} {layer2} < {value} TOLERANCE {num1} ABUT < 90 SINGULAR REGION
MinEnclosure_Inside——————————————————————————ENC {layer1} {layer2} < {value} ABUT < 90 SINGULAR INSIDE {layer3} REGION
MinEnclosure_Except——————————————————————————ENC {layer1} {layer2} < {value} ABUT < 90 SINGULAR EXCEPT {layer3} REGION
L1InsideL2——————————————————————————————     INside {layer1} {layer2}
L1InsideL2_Except——————————————————————————— INside {layer1} {layer2} EXCEPT {layer3}  
L1InsideL2_Inside——————————————————————————— INside {layer1} {layer2} INSIDE {layer3}
L1InteractL2—————————————————————————————INTERACT {layer1} {layer2}
L1InteractL2_Except——————————————————————————INTERACT {layer1} {layer2} EXCEPT {layer3}
L1InteractL2_Inside——————————————————————————INTERACT {layer1} {layer2} INSIDE {layer3}
FixedLengthByOrthogonal————————————————————————LENGTH {layer1} = {value} 
FixedLengthByOrthogonal_Except—————————————————————LENGTH {layer1} = {value} EXCEPT {layer3} 
FixedLengthByOrthogonal_Inside—————————————————————LENGTH {layer1} = {value} INSIDE {layer3}
MinDiameter—————————————————————————————DIAMETER {layer1} < {value} TOLERANCE {num1}
MinDiameter_Except——————————————————————————DIAMETER {layer1} < {value} TOLERANCE {num1}EXCEPT {layer3}
MinDiameter_Inside——————————————————————————DIAMETER {layer1} < {value} TOLERANCE {num1}INSIDE {layer3}
Density_Global_Max——————————————————————————DENSITY {layer1} > {value}
Density_Global_Min——————————————————————————DENSITY {layer1} < {value}
Density_Window_Max—————————————————————————DENSITY {layer1} WINDOW {num1} {num2} STEP {num3} > {value}
Density_Window_Min—————————————————————————DENSITY {layer1} WINDOW {num1} {num2} STEP {num3} < {value}
Density_Region_Max——————————————————————————DENSITY {layer1} EXCEPT {layer2} > {value}
Density_Region_Min——————————————————————————DENSITY {layer1} EXCEPT {layer2} < {value}
FixedOffset_XY————————————————————————————OFFSET {layer1} {num1} = {value}

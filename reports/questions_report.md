# Questions Test Report

- Generated: 2025-10-30 06:23:24Z
- Model: `/data/models/openai/gpt-oss-20b`
- CUDA devices: `2,3`
- Epochs: 1
- Samples: 10
- Similarity (avg/min/max): 13.51% / 2.52% / 23.10%

## Per-Question Results

| # | Similarity | Question | Final Answer (truncated) |
|---|------------|----------|--------------------------|
| q01 | 16.50% | 如何判定火灾的起火时间？ | 通过分析现场物证（如燃烧痕迹、烟熏模式）、证人证言和技术数据（如监控录像或碳化测试），综合推断火灾的起火时间范围。 |
| q02 | 2.52% | 起火原因鉴定的一般流程是什么？ | General process for fire cause identification: 1. Secure the scene and ensure safety. 2. Document the scene with phot... |
| q03 | 12.88% | 如何区分电气火灾与人为纵火？ | 通过电子数据优先分析时间线和异常，结合物证（熔珠、炭化、裂纹等）推断火势起源，交叉验证所有来源，系统排查电气故障与纵火迹象（如助燃剂、多点起火），重点部位解体取样，整合证据链并用排除法确认：电气火灾有局部过热、特定熔珠；人为纵火有助燃... |
| q04 | 9.88% | 如何采集并检测疑似加速剂（助燃剂）？ | 现场识别异味、渗透痕、多起火点；使用吸附片、注射器、密封罐采集炭化层、多孔材料、低处液体；实验室GC-MS分析挥发性有机物，检测汽油、柴油等加速剂特征峰；交叉验证电子日志与物证，排除其他原因，确认纵火。 |
| q05 | 23.10% | 现场勘查应拍摄与绘制哪些关键信息？ | 应拍摄：1) 现场全景与方位；2) 火源点及周边痕迹；3) 燃烧特征（炭化深度、烟熏层、玻璃裂纹）；4) 电气设备与线路状态；5) 可疑容器、助燃剂残留；6) 物证特写与比例尺。应绘制：1) 现场平面图（标注尺寸、物证位置）；2) 立... |
| q06 | 14.75% | 如何确保物证的保全与合法性？ | 为确保物证保全与合法性：1. 优先使用电子数据源（报警记录、监控、传感器日志）并交叉验证；2. 采样时选择焦化最深处，使用干净惰性容器（如油漆罐、金属罐），现场密封标识并建立完整流转链；3. 采用序列化拍摄（全景→中景→近景→细节），... |
| q07 | 12.28% | 如何评估自动消防系统（火灾报警与喷淋）的表现？ | 通过系统日志分析激活时间与响应延迟，结合现场喷淋覆盖、水流痕迹与火势物证交叉验证，评估系统及时性、有效性，识别故障原因并给出改进措施。 |
| q08 | 15.21% | 责任划分一般遵循哪些原则？ | 责任划分原则：1) 证据主导：电子数据与物证交叉验证确定起火原因与时间；2) 系统评估：检查消防设施联动、故障记录及设计符合性；3) 因果链分析：排除无关因素，锁定直接责任方；4) 程序合规：确保证据保全、流转链合法有效。 |
| q09 | 16.57% | 事故处置与善后一般包含哪些环节？ | 事故处置与善后包含四个核心环节：1) 应急响应与现场控制：启动应急预案、疏散人员、灭火救援、设立警戒线；2) 证据收集与调查：优先电子数据（监控、报警记录），整合物证分析，交叉验证时间线，保全证据链；3) 责任认定与法律处理：基于因果... |
| q10 | 11.37% | 如何将调查结论转化为可执行的预防改进措施？ | 将调查结论转化为可执行的预防改进措施：1) 制定涵盖人、机、料、法、环的全面整改计划，明确责任和时限；2) 组织复盘培训和应急演练，验证整改效果；3) 向监管部门提交改进报告并配合审查；4) 统一对外发布改进进展，应对舆情；5) 在改... |

## Detailed Findings

### q01 — Similarity 16.50%

**Question**

如何判定火灾的起火时间？

**Model Final Answer**

通过分析现场物证（如燃烧痕迹、烟熏模式）、证人证言和技术数据（如监控录像或碳化测试），综合推断火灾的起火时间范围。

**Reference Answer**

综合多源信息交叉印证：1) 报警/电话记录、监控时间戳、门禁与物联网传感器日志（烟感、温感、用电曲线）；2) 证人证言与值班交接记录；3) 物证迹象（熔珠、炭化深度、焦化边界、玻璃裂纹形态、烟熏层高度）推断火势发展阶段；4) 消防到场与控制时间倒推。以电子数据为主、物证为辅，相互校核得出时间窗口。

**Environment Feedback**

Similarity 16.50% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model provided a generic answer without specific technical methods or data sources, leading to low similarity with the ground truth. It missed critical electronic and forensic details.",
  "error_identification": "Omitted key technical data sources (e.g., electronic logs, sensor data, forensic markers) and failed to emphasize cross-verification.",
  "root_cause_analysis": "Relied on general knowledge without structured playbook guidance, resulting in incomplete and non-specific response.",
  "correct_approach": "Integrate electronic records (logs, sensors), forensic analysis (melting patterns, crack morphology), and cross-verify all sources to determine a precise time window.",
  "key_insight": "Always prioritize electronic data and multi-source cross-validation in time-sensitive forensic investigations.",
  "bullet_tags": []
}

**Curator Operations**

{
  "reasoning": "The reflection highlighted missing technical details and cross-verification in the response. The current playbook is empty, so new sections and bullets must be added based on the reflection's correct approach and key insight, aligning with the ground truth's emphasis on electronic data and multi-source validation.",
  "operations": [
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "优先使用电子数据源：报警/电话记录、监控时间戳、门禁与物联网传感器日志（烟感、温感、用电曲线）",
      "bullet_id": "electronic_data_priority",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "整合物证迹象分析：熔珠、炭化深度、焦化边界、玻璃裂纹形态、烟熏层高度以推断火势发展阶段",
      "bullet_id": "physical_evidence_analysis",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "交叉验证所有来源：电子数据为主、物证为辅，相互校核得出精确时间窗口",
      "bullet_id": "cross_verification",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "纳入证人证言与值班交接记录作为辅助时间参考",
      "bullet_id": "witness_records",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "利用消防到场与控制时间进行倒推分析",
      "bullet_id": "fire_control_timing",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q02 — Similarity 2.52%

**Question**

起火原因鉴定的一般流程是什么？

**Model Final Answer**

General process for fire cause identification: 1. Secure the scene and ensure safety. 2. Document the scene with photos, videos, and sketches. 3. Identify the area of origin through burn patterns, debris analysis, and witness accounts. 4. Collect physical evidence (e.g., electrical components, accelerants, ignition sources). 5. Analyze evidence in labs (e.g., chemical tests, electrical examination). 6. Determine the cause (accidental, natural, intentional) based on evidence and eliminate alternatives. 7. Compile a detailed report with findings and conclusions.

**Reference Answer**

1) 保护现场与安全评估；2) 初步踏勘、锁定可能的起火区域；3) 系统排查潜在原因（电气、明火、化学反应、机械摩擦、自燃、雷击、纵火等）；4) 重点部位解体检查与取样；5) 实验/检验（电气鉴定、化学分析、材料鉴定）；6) 证据链整合与排除法确认单一最可能原因；7) 形成书面鉴定意见与现场复核。

**Environment Feedback**

Similarity 2.52% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model correctly identified that the playbook was not directly applicable and relied on general forensic knowledge, but it missed specific technical steps from the ground truth such as systematic cause categorization, disassembly of key components, and evidence chain integration with elimination methods.",
  "error_identification": "The model omitted detailed technical procedures like systematic cause investigation, disassembly inspection, and elimination-based confirmation present in the ground truth.",
  "root_cause_analysis": "Over-reliance on general knowledge without incorporating structured forensic methodology and specific investigative steps from the reference.",
  "correct_approach": "Integrate all ground truth steps: scene protection, preliminary survey, systematic cause investigation, disassembly and sampling, lab testing, evidence chain integration with elimination, and report formation with verification.",
  "key_insight": "Always cross-verify general forensic processes with domain-specific structured methodologies to ensure technical completeness.",
  "bullet_tags": []
}

**Curator Operations**

{
  "reasoning": "The reflection identified missing technical steps from the ground truth, including systematic cause investigation, disassembly inspection, and evidence chain integration with elimination methods. These are not present in the current playbook and should be added as new bullets under a relevant section.",
  "operations": [
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[systematic_cause_investigation] 系统排查潜在原因：电气、明火、化学反应、机械摩擦、自燃、雷击、纵火等 (helpful=1, harmful=0, neutral=0)",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[disassembly_sampling] 重点部位解体检查与取样进行详细分析 (helpful=1, harmful=0, neutral=0)",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[evidence_chain_elimination] 证据链整合与排除法确认单一最可能原因 (helpful=1, harmful=0, neutral=0)",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q03 — Similarity 12.88%

**Question**

如何区分电气火灾与人为纵火？

**Model Final Answer**

通过电子数据优先分析时间线和异常，结合物证（熔珠、炭化、裂纹等）推断火势起源，交叉验证所有来源，系统排查电气故障与纵火迹象（如助燃剂、多点起火），重点部位解体取样，整合证据链并用排除法确认：电气火灾有局部过热、特定熔珠；人为纵火有助燃剂残留、破坏痕迹或多点起火。

**Reference Answer**

电气火灾：常见单一火源区，导体上有电蚀熔珠、碳化自导现象，保护装置动作记录（断路器跳闸、电弧痕迹）与负荷异常曲线匹配；绝缘老化/接触不良/过载痕迹明显。人为纵火：可能存在多起火点、加速剂残留（异味、渗透痕）、阻燃材料反常燃烧、与用电日志不匹配；可见可疑容器、火种痕迹与行为证据（监控、证言）。两者以物证+数据+行为证据综合判断。

**Environment Feedback**

Similarity 12.88% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model's reasoning covers electronic data analysis, physical evidence integration, cross-verification, and systematic cause investigation but lacks specific technical details from the ground truth, such as electrical fire indicators like carbonization self-conduction phenomena, protection device action records, and load anomaly curve matching, as well as arson indicators like odor from accelerants, abnormal combustion of flame-retardant materials, and mismatch with electricity logs. The divergence stems from insufficient incorporation of these precise diagnostic markers.",
  "error_identification": "The model omitted key technical details from the ground truth, including specific electrical fire signs (e.g., carbonization self-conduction, protection device actions, load anomalies) and arson indicators (e.g., accelerant odors, abnormal flame-retardant material combustion, electricity log mismatches), leading to low similarity and incomplete differentiation criteria.",
  "root_cause_analysis": "The model relied on general investigation steps without integrating the nuanced, evidence-based technical markers provided in the ground truth, resulting in a divergent and less precise prediction that fails to capture the full diagnostic spectrum required for accurate fire cause determination.",
  "correct_approach": "Incorporate the missing technical details: for electrical fires, include carbonization self-conduction, protection device action records (e.g., circuit breaker trips, arc traces), and load anomaly curve matching; for arson, include accelerant residues (odors, penetration marks), abnormal combustion of flame-retardant materials, and inconsistencies with electricity logs, while maintaining systematic evidence integration and cross-verification.",
  "key_insight": "Accurate fire cause differentiation requires not only systematic investigation steps but also the integration of specific, evidence-based technical markers—such as electrical protection device records and accelerant detection—to ensure precision and avoid divergence from established diagnostic criteria.",
  "bullet_tags": [
    {
      "id": "electronic_data_priority",
      "tag": "helpful"
    },
    {
      "id": "physical_evidence_analysis",
      "tag": "helpful"
    },
    {
      "id": "cross_verification",
      "tag": "helpful"
    },
    {
      "id": "systematic_cause_investigation",
      "tag": "helpful"
    },
    {
      "id": "disassembly_sampling",
      "tag": "helpful"
    },
    {
      "id": "evidence_chain_elimination",
      "tag": "helpful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identifies missing technical details for differentiating electrical fires from arson, including specific electrical indicators (carbonization self-conduction, protection device actions, load anomalies) and arson indicators (accelerant residues, abnormal combustion of flame-retardant materials, electricity log mismatches). These are absent in the current playbook and must be added to improve diagnostic precision.",
  "operations": [
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[electrical_fire_indicators] 电气火灾特征：单一火源区，导体上电蚀熔珠、碳化自导现象，保护装置动作记录（断路器跳闸、电弧痕迹）与负荷异常曲线匹配，绝缘老化/接触不良/过载痕迹明显",
      "bullet_id": "electrical_fire_indicators",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[arson_indicators] 人为纵火特征：多起火点可能，加速剂残留（异味、渗透痕）、阻燃材料反常燃烧、与用电日志不匹配，可疑容器、火种痕迹与行为证据（监控、证言）",
      "bullet_id": "arson_indicators",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q04 — Similarity 9.88%

**Question**

如何采集并检测疑似加速剂（助燃剂）？

**Model Final Answer**

现场识别异味、渗透痕、多起火点；使用吸附片、注射器、密封罐采集炭化层、多孔材料、低处液体；实验室GC-MS分析挥发性有机物，检测汽油、柴油等加速剂特征峰；交叉验证电子日志与物证，排除其他原因，确认纵火。

**Reference Answer**

采样：选择焦化最深处及下渗位置，用干净惰性容器（油漆罐/专用金属罐或活性炭管），现场密封标识并建立流转链；避免交叉污染与挥发损失。检测：顶空/动态顶空→GC-MS；必要时FTIR或GC-FID复核；与空白样和参比谱库比对。结果需结合现场合理解释（例如车辆泄漏燃油 vs. 故意泼洒）。

**Environment Feedback**

Similarity 9.88% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model's response was overly general and omitted critical technical details from the ground truth, such as specific sampling containers (clean inert containers like paint cans or metal cans, activated carbon tubes), proper chain of custody, and advanced detection methods (headspace/dynamic headspace GC-MS, FTIR or GC-FID for verification). It also failed to emphasize the importance of comparing samples with blanks and reference libraries and providing contextual interpretation of results.",
  "error_identification": "The model omitted key technical specifications for sampling (e.g., clean inert containers, chain of custody) and detection methods (e.g., headspace techniques, verification with FTIR/GC-FID, comparison with blanks and reference libraries). It also lacked emphasis on contextual result interpretation.",
  "root_cause_analysis": "The model relied on a high-level summary without incorporating detailed procedural steps from the ground truth, leading to a divergent response with low similarity. It prioritized brevity over technical accuracy and completeness.",
  "correct_approach": "Specify sampling with clean inert containers (paint cans, metal cans, activated carbon tubes), ensure proper sealing, labeling, and chain of custody. Use headspace or dynamic headspace with GC-MS for analysis, verify with FTIR or GC-FID if needed, compare with blank samples and reference libraries, and interpret results in context (e.g., distinguishing accidental leaks from intentional pouring).",
  "key_insight": "Accelerant detection requires precise sampling protocols, advanced analytical techniques with verification steps, and contextual interpretation to avoid misclassification.",
  "bullet_tags": [
    {
      "id": "sampling_containers",
      "tag": "helpful"
    },
    {
      "id": "chain_of_custody",
      "tag": "helpful"
    },
    {
      "id": "headspace_techniques",
      "tag": "helpful"
    },
    {
      "id": "verification_methods",
      "tag": "helpful"
    },
    {
      "id": "contextual_interpretation",
      "tag": "helpful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identifies missing technical details in the current playbook regarding accelerant detection, including specific sampling containers, chain of custody, analytical methods, verification steps, and contextual interpretation. These elements are critical for accurate accelerant detection and are not covered in the existing 'arson_indicators' bullet.",
  "operations": [
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[accelerant_detection] 采样：选择焦化最深处及下渗位置，使用干净惰性容器（油漆罐、专用金属罐或活性炭管），现场密封标识并建立流转链；避免交叉污染与挥发损失。检测：顶空/动态顶空→GC-MS；必要时FTIR或GC-FID复核；与空白样和参比谱库比对。结果需结合现场合理解释（例如车辆泄漏燃油 vs. 故意泼洒）。",
      "bullet_id": "accelerant_detection",
      "metadata": {
        "helpful": 5,
        "harmful": 0
      }
    }
  ]
}

### q05 — Similarity 23.10%

**Question**

现场勘查应拍摄与绘制哪些关键信息？

**Model Final Answer**

应拍摄：1) 现场全景与方位；2) 火源点及周边痕迹；3) 燃烧特征（炭化深度、烟熏层、玻璃裂纹）；4) 电气设备与线路状态；5) 可疑容器、助燃剂残留；6) 物证特写与比例尺。应绘制：1) 现场平面图（标注尺寸、物证位置）；2) 立体示意图（火势蔓延路径）；3) 痕迹分布图（焦化边界、多火点位置）。

**Reference Answer**

照片：全景→中景→近景→细节的序列；标注方位、比例尺与编号；记录火舌方向、烟熏界线、倒伏痕迹、喷淋头启动状况、配电箱状态等。草图/示意图：平面图与剖面图，标注起火区、火势蔓延路径、开口部位、可燃物堆码、消防设施位置与编号；必要时激光测距标注尺寸与北向。

**Environment Feedback**

Similarity 23.10% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model's response lists key items to photograph and draw but lacks systematic sequencing, specific technical markers, and integration of forensic analysis. It omits critical details like fire plume direction, smoke demarcation, collapse patterns, sprinkler status, and precise dimensional annotations. The ground truth emphasizes a structured progression from wide to detailed shots and includes technical measurements and forensic markers for fire behavior analysis.",
  "error_identification": "The model provided a generic list without the structured sequence (panorama to detail), omitted key forensic indicators (fire plume direction, smoke boundaries, collapse traces, sprinkler activation), and missed precise technical annotations (laser measurements, north orientation, numbering).",
  "root_cause_analysis": "Over-reliance on high-level categories without integrating systematic forensic protocols or referencing specific technical standards for fire scene documentation led to omission of sequential imaging, measurable annotations, and behavioral fire indicators.",
  "correct_approach": "Follow a sequential imaging protocol: panorama → mid-range → close-up → detail shots, each with scale, orientation, and numbering. Include fire behavior indicators (plume direction, smoke lines, collapse patterns, sprinkler status). Draw annotated plans and sections with起火区, spread paths, openings, combustibles, fire protection features, and laser-measured dimensions with north arrow.",
  "key_insight": "Fire scene documentation must combine a systematic visual sequence with measurable forensic markers (plume, smoke, collapse) and annotated diagrams integrating spatial, behavioral, and physical evidence for accurate fire origin and progression analysis.",
  "bullet_tags": [
    {
      "id": "sequence_imaging",
      "tag": "helpful"
    },
    {
      "id": "forensic_indicators",
      "tag": "helpful"
    },
    {
      "id": "annotated_diagrams",
      "tag": "helpful"
    },
    {
      "id": "generic_listing",
      "tag": "harmful"
    },
    {
      "id": "missing_measurements",
      "tag": "harmful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identifies missing systematic sequencing, forensic indicators, and technical annotations in fire scene documentation. The current playbook lacks a section on scene documentation, so new bullets are added to incorporate the structured imaging protocol, forensic markers, and annotated diagrams from the reflection and ground truth.",
  "operations": [
    {
      "type": "ADD",
      "section": "现场勘查拍摄与绘制",
      "content": "[sequence_imaging] 采用序列化拍摄：全景→中景→近景→细节，每张照片标注方位、比例尺与编号",
      "bullet_id": "sequence_imaging",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "现场勘查拍摄与绘制",
      "content": "[forensic_indicators] 记录火舌方向、烟熏界线、倒伏痕迹、喷淋头启动状况、配电箱状态等火灾行为与痕迹指标",
      "bullet_id": "forensic_indicators",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "现场勘查拍摄与绘制",
      "content": "[annotated_diagrams] 绘制平面图与剖面图，标注起火区、火势蔓延路径、开口部位、可燃物堆码、消防设施位置与编号；必要时激光测距标注尺寸与北向",
      "bullet_id": "annotated_diagrams",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q06 — Similarity 14.75%

**Question**

如何确保物证的保全与合法性？

**Model Final Answer**

为确保物证保全与合法性：1. 优先使用电子数据源（报警记录、监控、传感器日志）并交叉验证；2. 采样时选择焦化最深处，使用干净惰性容器（如油漆罐、金属罐），现场密封标识并建立完整流转链；3. 采用序列化拍摄（全景→中景→近景→细节），每张照片标注方位、比例尺与编号；4. 记录火舌方向、烟熏界线等火灾行为指标；5. 绘制平面图与剖面图，标注起火区、火势蔓延路径等关键信息；6. 系统排查原因，整合证据链与排除法确认最可能原因。

**Reference Answer**

1) 现场设警戒和单一出入口，建立进出清单；2) 物证编号、拍照、记录采集位置与条件；3) 使用封签并填写取证单与流转链（时间、人员、目的、条件）；4) 易挥发/腐蚀/含水样品分类储存（低温、避光、密封）；5) 运输与实验室接收双人交接签字；6) 全程留痕可追溯，避免“污染、丢失、替换、无法解释”的风险。

**Environment Feedback**

Similarity 14.75% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model focused on technical sampling and imaging procedures but missed foundational legal and chain-of-custody protocols essential for evidence admissibility.",
  "error_identification": "Omitted critical legal safeguards: no access control, evidence labeling, custody documentation, or specialized storage protocols.",
  "root_cause_analysis": "Over-reliance on technical playbook excerpts without integrating legal/forensic standards for evidence integrity.",
  "correct_approach": "Combine technical procedures with legal chain-of-custody: secure scene, document evidence transfers, use tamper-proof seals, and implement dual-person verification.",
  "key_insight": "Technical accuracy alone is insufficient; evidence must be legally defensible through documented custody and contamination prevention.",
  "bullet_tags": [
    {
      "id": "electronic_data_priority",
      "tag": "helpful"
    },
    {
      "id": "accelerant_detection",
      "tag": "helpful"
    },
    {
      "id": "sequence_imaging",
      "tag": "helpful"
    },
    {
      "id": "missing_chain_of_custody",
      "tag": "harmful"
    },
    {
      "id": "missing_legal_documentation",
      "tag": "harmful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identified missing legal and chain-of-custody protocols for evidence integrity. The reference answer provided specific technical details for evidence preservation and legality, which were not present in the current playbook. Added a new section '物证保全与合法性' with structured bullets covering scene control, evidence documentation, chain-of-custody, storage, transport, and traceability to address these gaps.",
  "operations": [
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[scene_control] 现场设警戒线和单一出入口，建立进出人员与物品清单，防止未经授权进入",
      "bullet_id": "scene_control",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[evidence_documentation] 物证编号、拍照、记录采集位置、时间、环境条件与采集人员",
      "bullet_id": "evidence_documentation",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[chain_of_custody] 使用封签并填写取证单与流转链，记录每次交接的时间、人员、目的和存储条件",
      "bullet_id": "chain_of_custody",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[specialized_storage] 易挥发、腐蚀性或含水样品分类储存，采用低温、避光、密封容器防止变质或污染",
      "bullet_id": "specialized_storage",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[dual_verification_transport] 运输与实验室接收实行双人交接签字，确保证据转移的可控性与责任明确",
      "bullet_id": "dual_verification_transport",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "物证保全与合法性",
      "content": "[traceability_prevention] 全程留痕可追溯，严格避免污染、丢失、替换或无法解释的风险，确保证据法律效力",
      "bullet_id": "traceability_prevention",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q07 — Similarity 12.28%

**Question**

如何评估自动消防系统（火灾报警与喷淋）的表现？

**Model Final Answer**

通过系统日志分析激活时间与响应延迟，结合现场喷淋覆盖、水流痕迹与火势物证交叉验证，评估系统及时性、有效性，识别故障原因并给出改进措施。

**Reference Answer**

对照设计与维保记录，核对：1) 报警触发顺序与时间（探测器、手报、联动）；2) 喷淋启动时间、开启喷头数量与覆盖区域、水流/压力记录；3) 防火分区与防火门/排烟系统联动是否到位；4) 近期故障/屏蔽/停用记录；5) 现场残留迹象（启动指示、湿度、冲刷痕）；将实际表现与规范/设计目标对比，判断系统对控制火势的贡献与缺陷。

**Environment Feedback**

Similarity 12.28% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model's reasoning focused on general steps for evaluating system performance but missed critical technical details from the ground truth, such as specific verification of alarm trigger sequences, fire compartment and door/smoke exhaust system linkages, recent fault records, and comparison with design specifications. The feedback indicated divergence (12.28% similarity), highlighting the omission of these elements.",
  "error_identification": "The model failed to incorporate key technical details from the ground truth, including alarm trigger order verification, fire compartment and smoke system linkage checks, recent fault/disablement records, and design specification comparisons.",
  "root_cause_analysis": "The model relied on a generic evaluation framework without integrating the precise, structured verification steps and technical cross-checks specified in the reference answer, leading to a superficial analysis.",
  "correct_approach": "Adopt a structured verification approach: 1) Verify alarm trigger sequence and timing (detectors, manual alarms, linkages); 2) Check sprinkler activation time, number of activated heads, coverage area, and water flow/pressure records; 3) Assess fire compartment and door/smoke exhaust system linkages; 4) Review recent fault/shutdown/disablement logs; 5) Examine physical evidence (activation indicators, humidity, wash marks); 6) Compare actual performance with design standards to evaluate system contribution and defects.",
  "key_insight": "Effective evaluation requires cross-verifying electronic data (logs, sensors) with physical evidence and design specifications, ensuring all technical components (alarm sequences, system linkages, maintenance records) are systematically checked against standards.",
  "bullet_tags": [
    {
      "id": "alarm_sequence",
      "tag": "helpful"
    },
    {
      "id": "sprinkler_coverage",
      "tag": "helpful"
    },
    {
      "id": "system_linkage",
      "tag": "helpful"
    },
    {
      "id": "fault_records",
      "tag": "helpful"
    },
    {
      "id": "design_comparison",
      "tag": "helpful"
    },
    {
      "id": "generic_framework",
      "tag": "harmful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identifies missing technical details in evaluating automatic fire protection systems, including alarm sequence verification, sprinkler coverage, system linkages, fault records, and design comparisons. These elements are not present in the current playbook and should be added as new bullets under a relevant section.",
  "operations": [
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[alarm_sequence] 验证报警触发顺序与时间：核对探测器、手动报警、联动设备的触发顺序与时间记录",
      "bullet_id": "alarm_sequence",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[sprinkler_coverage] 检查喷淋启动时间、开启喷头数量、覆盖区域、水流与压力记录",
      "bullet_id": "sprinkler_coverage",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[system_linkage] 评估防火分区与防火门/排烟系统联动是否到位",
      "bullet_id": "system_linkage",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[fault_records] 审查近期故障、屏蔽、停用记录",
      "bullet_id": "fault_records",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[design_comparison] 将实际表现与规范/设计目标对比，判断系统对控制火势的贡献与缺陷",
      "bullet_id": "design_comparison",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "火灾起火时间判定",
      "content": "[generic_framework] 避免使用通用评估框架，应整合具体技术细节与交叉验证步骤",
      "bullet_id": "generic_framework",
      "metadata": {
        "helpful": 0,
        "harmful": 1
      }
    }
  ]
}

### q08 — Similarity 15.21%

**Question**

责任划分一般遵循哪些原则？

**Model Final Answer**

责任划分原则：1) 证据主导：电子数据与物证交叉验证确定起火原因与时间；2) 系统评估：检查消防设施联动、故障记录及设计符合性；3) 因果链分析：排除无关因素，锁定直接责任方；4) 程序合规：确保证据保全、流转链合法有效。

**Reference Answer**

依据当地消防、安全生产、民刑事法律法规及合同：1) 因果关系与过错责任为核心（直接原因方承担主责）；2) 管理控制义务与维保义务未履行构成管理过错（如物业、用人单位、承包方）；3) 违法行为（违规动火、私拉乱接、擅自停用消防设施）从重；4) 纵火等故意犯罪移送刑事；5) 多方过错按过错比例分担民事赔偿。

**Environment Feedback**

Similarity 15.21% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model focused excessively on technical evidence collection and verification procedures, missing the core legal and liability principles that govern responsibility allocation. It failed to incorporate fundamental legal concepts such as fault liability, management obligations, illegal acts, criminal intent, and proportional liability sharing.",
  "error_identification": "Model omitted essential legal framework elements including fault-based liability, management control obligations, illegal acts, criminal liability, and proportional fault allocation.",
  "root_cause_analysis": "Over-reliance on technical evidence procedures without integrating the legal principles that actually determine responsibility allocation in liability cases.",
  "correct_approach": "Combine technical evidence analysis with legal liability principles: establish causation and fault as core, identify management and maintenance obligations, flag illegal acts and criminal behavior, and determine proportional liability for multiple parties.",
  "key_insight": "Technical evidence serves legal liability determination - evidence procedures must be framed within the legal principles that actually govern responsibility allocation.",
  "bullet_tags": [
    {
      "id": "electronic_data_priority",
      "tag": "helpful"
    },
    {
      "id": "physical_evidence_analysis",
      "tag": "helpful"
    },
    {
      "id": "cross_verification",
      "tag": "helpful"
    },
    {
      "id": "system_linkage",
      "tag": "neutral"
    },
    {
      "id": "fault_records",
      "tag": "neutral"
    },
    {
      "id": "design_comparison",
      "tag": "neutral"
    },
    {
      "id": "chain_of_custody",
      "tag": "helpful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection identified a critical gap in the playbook: missing legal liability principles that govern responsibility allocation. The current playbook focuses heavily on technical evidence procedures but lacks integration with legal frameworks. The reference answer and ground truth provide clear legal principles that must be incorporated. I will add a new section specifically for legal liability principles, combining elements from the reflection's correct approach and the ground truth.",
  "operations": [
    {
      "type": "ADD",
      "section": "法律责任划分原则",
      "content": "[causation_fault_core] 因果关系与过错责任为核心：确定直接原因方承担主要责任，基于证据链建立因果联系与过错事实",
      "bullet_id": "causation_fault_core",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "法律责任划分原则",
      "content": "[management_obligations] 管理控制义务与维保义务：物业、用人单位、承包方等未履行管理控制与维护保养义务构成管理过错",
      "bullet_id": "management_obligations",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "法律责任划分原则",
      "content": "[illegal_acts_emphasis] 违法行为从重处理：违规动火、私拉乱接电线、擅自停用消防设施等违法行为需从严认定责任",
      "bullet_id": "illegal_acts_emphasis",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "法律责任划分原则",
      "content": "[criminal_liability] 故意犯罪移送刑事：纵火等故意犯罪行为需移送刑事司法程序处理",
      "bullet_id": "criminal_liability",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "法律责任划分原则",
      "content": "[proportional_liability] 多方过错按比例分担：存在多个责任方时，根据过错程度按比例分担民事赔偿责任",
      "bullet_id": "proportional_liability",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q09 — Similarity 16.57%

**Question**

事故处置与善后一般包含哪些环节？

**Model Final Answer**

事故处置与善后包含四个核心环节：1) 应急响应与现场控制：启动应急预案、疏散人员、灭火救援、设立警戒线；2) 证据收集与调查：优先电子数据（监控、报警记录），整合物证分析，交叉验证时间线，保全证据链；3) 责任认定与法律处理：基于因果关系和过错确定责任方，审查管理义务履行情况，处理违法行为，按比例分担责任，涉嫌犯罪移送司法；4) 善后恢复：损失评估、保险理赔、系统修复、整改措施落实。

**Reference Answer**

1) 现场清理与结构安全评估；2) 暂停相关作业，制定临时防护与复工条件；3) 伤亡救助与心理支持；4) 保险报案、损失评估、资料归档；5) 与监管部门沟通并提交调查报告；6) 对外信息发布与舆情应对；7) 整改计划（人、机、料、法、环）与时限；8) 复盘培训与演练，关闭整改项并复核效果。

**Environment Feedback**

Similarity 16.57% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "The model focused heavily on legal and technical investigation aspects from the playbook, such as causation, fault determination, evidence collection, and liability, but overlooked practical emergency response, victim support, regulatory communication, and recovery steps present in the ground truth.",
  "error_identification": "The model omitted critical phases like victim care, regulatory reporting, public communication, and corrective action implementation, leading to low similarity with the ground truth.",
  "root_cause_analysis": "Over-reliance on playbook excerpts about investigation and liability, without integrating broader accident management phases such as immediate humanitarian response and post-incident recovery.",
  "correct_approach": "Combine investigation and liability steps from the playbook with ground truth elements: include victim rescue, psychological support, regulatory communication, public information management, and systematic corrective planning.",
  "key_insight": "Accident handling must balance investigation/liability with immediate humanitarian and operational recovery steps; use playbook for technical details but ensure comprehensive phase coverage.",
  "bullet_tags": [
    {
      "id": "causation_fault_core",
      "tag": "helpful"
    },
    {
      "id": "electronic_data_priority",
      "tag": "helpful"
    },
    {
      "id": "scene_control",
      "tag": "helpful"
    },
    {
      "id": "management_obligations",
      "tag": "neutral"
    },
    {
      "id": "illegal_acts_emphasis",
      "tag": "neutral"
    },
    {
      "id": "proportional_liability",
      "tag": "neutral"
    },
    {
      "id": "missing_victim_support",
      "tag": "harmful"
    },
    {
      "id": "missing_regulatory_reporting",
      "tag": "harmful"
    },
    {
      "id": "missing_corrective_actions",
      "tag": "harmful"
    }
  ]
}

**Curator Operations**

{
  "operations": [
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[victim_support] 伤亡救助与心理支持：立即组织医疗救援，提供急救与心理疏导服务，确保伤亡人员得到及时关怀与后续支持",
      "bullet_id": "victim_support",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[regulatory_reporting] 与监管部门沟通并提交调查报告：及时向相关监管机构报告事故情况，按要求提交详细调查报告，配合审查与指导",
      "bullet_id": "regulatory_reporting",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[corrective_actions] 整改计划（人、机、料、法、环）与时限：制定全面整改方案，涵盖人员、设备、材料、方法、环境等方面，明确实施时限与责任分工",
      "bullet_id": "corrective_actions",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[public_communication] 对外信息发布与舆情应对：统一信息发布口径，及时公开事故处理进展，监测并应对舆情，维护公众信任",
      "bullet_id": "public_communication",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[site_recovery] 现场清理与结构安全评估：清理事故现场，评估建筑结构安全，确保无次生风险后恢复基本环境",
      "bullet_id": "site_recovery",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[temporary_measures] 暂停相关作业，制定临时防护与复工条件：立即停止危险作业，设立临时安全防护措施，明确复工前必须满足的安全条件",
      "bullet_id": "temporary_measures",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[insurance_documentation] 保险报案、损失评估、资料归档：及时向保险公司报案，评估财产与责任损失，系统整理并归档所有事故相关文件",
      "bullet_id": "insurance_documentation",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    },
    {
      "type": "ADD",
      "section": "事故处置与善后",
      "content": "[review_training] 复盘培训与演练，关闭整改项并复核效果：组织事故复盘会议，开展针对性培训与应急演练，确保整改措施落实并验证其有效性",
      "bullet_id": "review_training",
      "metadata": {
        "helpful": 1,
        "harmful": 0
      }
    }
  ]
}

### q10 — Similarity 11.37%

**Question**

如何将调查结论转化为可执行的预防改进措施？

**Model Final Answer**

将调查结论转化为可执行的预防改进措施：1) 制定涵盖人、机、料、法、环的全面整改计划，明确责任和时限；2) 组织复盘培训和应急演练，验证整改效果；3) 向监管部门提交改进报告并配合审查；4) 统一对外发布改进进展，应对舆情；5) 在改进期间实施临时安全防护措施，明确复工条件。

**Reference Answer**

依据根因分析制定“问题-措施-责任-时限-KPI”闭环：电气类→增设回路保护、红外测温巡检、更新老化线缆；管理类→动火许可/监护、危化品分区与台账、堆码高度与通道管理；工程类→防火分隔与封堵、耐火等级提升、排烟与应急照明优化；人员类→分级培训与实操演练；监控类→增加视频/用电/环境传感器并联动预警；定期内审与第三方复评。

**Environment Feedback**

Similarity 11.37% -> divergent. If divergent, incorporate missing technical details from the reference answer.

**Reflection Snapshot**

{
  "reasoning": "Model prediction omitted technical specifics from ground truth, such as electrical protections, fire management, engineering upgrades, and monitoring systems, leading to low similarity. It followed a generic corrective action framework without incorporating root cause analysis or measurable KPIs.",
  "error_identification": "Missing technical details and failure to link corrective actions to specific root causes; absence of KPI-based validation and engineering controls.",
  "root_cause_analysis": "Over-reliance on generic playbook steps without adapting to the detailed ground truth; insufficient integration of root cause analysis into actionable, measurable items.",
  "correct_approach": "Map each root cause (electrical, management, engineering, personnel, monitoring) to specific corrective actions with clear responsibilities, timelines, and KPIs; include technical measures like circuit protection, fire separation, sensor systems, and periodic audits.",
  "key_insight": "Preventive measures must be derived directly from root cause analysis with technical specificity and closed-loop validation (problem-measure-responsibility-timeline-KPI).",
  "bullet_tags": [
    {
      "id": "corrective_actions",
      "tag": "helpful"
    },
    {
      "id": "review_training",
      "tag": "helpful"
    },
    {
      "id": "regulatory_reporting",
      "tag": "neutral"
    },
    {
      "id": "public_communication",
      "tag": "neutral"
    },
    {
      "id": "temporary_measures",
      "tag": "helpful"
    }
  ]
}

**Curator Operations**

{
  "reasoning": "The reflection highlighted the need for technical specificity and a closed-loop corrective action framework derived from root cause analysis. The current playbook lacks detailed mapping of root causes to specific technical measures, responsibilities, timelines, and KPIs. The reference answer provides concrete examples of such measures across electrical, management, engineering, personnel, and monitoring categories. These should be integrated into the corrective actions section to enhance specificity and measurability.",
  "operations": [
    {
      "type": "UPDATE",
      "section": "事故处置与善后",
      "content": "整改计划（人、机、料、法、环）与时限：依据根因分析制定“问题-措施-责任-时限-KPI”闭环：电气类→增设回路保护、红外测温巡检、更新老化线缆；管理类→动火许可/监护、危化品分区与台账、堆码高度与通道管理；工程类→防火分隔与封堵、耐火等级提升、排烟与应急照明优化；人员类→分级培训与实操演练；监控类→增加视频/用电/环境传感器并联动预警；定期内审与第三方复评。",
      "bullet_id": "corrective_actions",
      "metadata": {
        "helpful": 3,
        "harmful": 0
      }
    }
  ]
}

## Final Playbook

## 事故处置与善后
- [victim_support] [victim_support] 伤亡救助与心理支持：立即组织医疗救援，提供急救与心理疏导服务，确保伤亡人员得到及时关怀与后续支持 (helpful=1, harmful=0, neutral=0)
- [regulatory_reporting] [regulatory_reporting] 与监管部门沟通并提交调查报告：及时向相关监管机构报告事故情况，按要求提交详细调查报告，配合审查与指导 (helpful=1, harmful=0, neutral=1)
- [corrective_actions] 整改计划（人、机、料、法、环）与时限：依据根因分析制定“问题-措施-责任-时限-KPI”闭环：电气类→增设回路保护、红外测温巡检、更新老化线缆；管理类→动火许可/监护、危化品分区与台账、堆码高度与通道管理；工程类→防火分隔与封堵、耐火等级提升、排烟与应急照明优化；人员类→分级培训与实操演练；监控类→增加视频/用电/环境传感器并联动预警；定期内审与第三方复评。 (helpful=3, harmful=0, neutral=0)
- [public_communication] [public_communication] 对外信息发布与舆情应对：统一信息发布口径，及时公开事故处理进展，监测并应对舆情，维护公众信任 (helpful=1, harmful=0, neutral=1)
- [site_recovery] [site_recovery] 现场清理与结构安全评估：清理事故现场，评估建筑结构安全，确保无次生风险后恢复基本环境 (helpful=1, harmful=0, neutral=0)
- [temporary_measures] [temporary_measures] 暂停相关作业，制定临时防护与复工条件：立即停止危险作业，设立临时安全防护措施，明确复工前必须满足的安全条件 (helpful=2, harmful=0, neutral=0)
- [insurance_documentation] [insurance_documentation] 保险报案、损失评估、资料归档：及时向保险公司报案，评估财产与责任损失，系统整理并归档所有事故相关文件 (helpful=1, harmful=0, neutral=0)
- [review_training] [review_training] 复盘培训与演练，关闭整改项并复核效果：组织事故复盘会议，开展针对性培训与应急演练，确保整改措施落实并验证其有效性 (helpful=2, harmful=0, neutral=0)
## 法律责任划分原则
- [causation_fault_core] [causation_fault_core] 因果关系与过错责任为核心：确定直接原因方承担主要责任，基于证据链建立因果联系与过错事实 (helpful=2, harmful=0, neutral=0)
- [management_obligations] [management_obligations] 管理控制义务与维保义务：物业、用人单位、承包方等未履行管理控制与维护保养义务构成管理过错 (helpful=1, harmful=0, neutral=1)
- [illegal_acts_emphasis] [illegal_acts_emphasis] 违法行为从重处理：违规动火、私拉乱接电线、擅自停用消防设施等违法行为需从严认定责任 (helpful=1, harmful=0, neutral=1)
- [criminal_liability] [criminal_liability] 故意犯罪移送刑事：纵火等故意犯罪行为需移送刑事司法程序处理 (helpful=1, harmful=0, neutral=0)
- [proportional_liability] [proportional_liability] 多方过错按比例分担：存在多个责任方时，根据过错程度按比例分担民事赔偿责任 (helpful=1, harmful=0, neutral=1)
## 火灾起火时间判定
- [electronic_data_priority] 优先使用电子数据源：报警/电话记录、监控时间戳、门禁与物联网传感器日志（烟感、温感、用电曲线） (helpful=5, harmful=0, neutral=0)
- [physical_evidence_analysis] 整合物证迹象分析：熔珠、炭化深度、焦化边界、玻璃裂纹形态、烟熏层高度以推断火势发展阶段 (helpful=3, harmful=0, neutral=0)
- [cross_verification] 交叉验证所有来源：电子数据为主、物证为辅，相互校核得出精确时间窗口 (helpful=3, harmful=0, neutral=0)
- [witness_records] 纳入证人证言与值班交接记录作为辅助时间参考 (helpful=1, harmful=0, neutral=0)
- [fire_control_timing] 利用消防到场与控制时间进行倒推分析 (helpful=1, harmful=0, neutral=0)
- [火灾起火时间判定-00001] [systematic_cause_investigation] 系统排查潜在原因：电气、明火、化学反应、机械摩擦、自燃、雷击、纵火等 (helpful=1, harmful=0, neutral=0) (helpful=1, harmful=0, neutral=0)
- [火灾起火时间判定-00002] [disassembly_sampling] 重点部位解体检查与取样进行详细分析 (helpful=1, harmful=0, neutral=0) (helpful=1, harmful=0, neutral=0)
- [火灾起火时间判定-00003] [evidence_chain_elimination] 证据链整合与排除法确认单一最可能原因 (helpful=1, harmful=0, neutral=0) (helpful=1, harmful=0, neutral=0)
- [electrical_fire_indicators] [electrical_fire_indicators] 电气火灾特征：单一火源区，导体上电蚀熔珠、碳化自导现象，保护装置动作记录（断路器跳闸、电弧痕迹）与负荷异常曲线匹配，绝缘老化/接触不良/过载痕迹明显 (helpful=1, harmful=0, neutral=0)
- [arson_indicators] [arson_indicators] 人为纵火特征：多起火点可能，加速剂残留（异味、渗透痕）、阻燃材料反常燃烧、与用电日志不匹配，可疑容器、火种痕迹与行为证据（监控、证言） (helpful=1, harmful=0, neutral=0)
- [accelerant_detection] [accelerant_detection] 采样：选择焦化最深处及下渗位置，使用干净惰性容器（油漆罐、专用金属罐或活性炭管），现场密封标识并建立流转链；避免交叉污染与挥发损失。检测：顶空/动态顶空→GC-MS；必要时FTIR或GC-FID复核；与空白样和参比谱库比对。结果需结合现场合理解释（例如车辆泄漏燃油 vs. 故意泼洒）。 (helpful=6, harmful=0, neutral=0)
- [alarm_sequence] [alarm_sequence] 验证报警触发顺序与时间：核对探测器、手动报警、联动设备的触发顺序与时间记录 (helpful=1, harmful=0, neutral=0)
- [sprinkler_coverage] [sprinkler_coverage] 检查喷淋启动时间、开启喷头数量、覆盖区域、水流与压力记录 (helpful=1, harmful=0, neutral=0)
- [system_linkage] [system_linkage] 评估防火分区与防火门/排烟系统联动是否到位 (helpful=1, harmful=0, neutral=1)
- [fault_records] [fault_records] 审查近期故障、屏蔽、停用记录 (helpful=1, harmful=0, neutral=1)
- [design_comparison] [design_comparison] 将实际表现与规范/设计目标对比，判断系统对控制火势的贡献与缺陷 (helpful=1, harmful=0, neutral=1)
- [generic_framework] [generic_framework] 避免使用通用评估框架，应整合具体技术细节与交叉验证步骤 (helpful=0, harmful=1, neutral=0)
## 物证保全与合法性
- [scene_control] [scene_control] 现场设警戒线和单一出入口，建立进出人员与物品清单，防止未经授权进入 (helpful=2, harmful=0, neutral=0)
- [evidence_documentation] [evidence_documentation] 物证编号、拍照、记录采集位置、时间、环境条件与采集人员 (helpful=1, harmful=0, neutral=0)
- [chain_of_custody] [chain_of_custody] 使用封签并填写取证单与流转链，记录每次交接的时间、人员、目的和存储条件 (helpful=2, harmful=0, neutral=0)
- [specialized_storage] [specialized_storage] 易挥发、腐蚀性或含水样品分类储存，采用低温、避光、密封容器防止变质或污染 (helpful=1, harmful=0, neutral=0)
- [dual_verification_transport] [dual_verification_transport] 运输与实验室接收实行双人交接签字，确保证据转移的可控性与责任明确 (helpful=1, harmful=0, neutral=0)
- [traceability_prevention] [traceability_prevention] 全程留痕可追溯，严格避免污染、丢失、替换或无法解释的风险，确保证据法律效力 (helpful=1, harmful=0, neutral=0)
## 现场勘查拍摄与绘制
- [sequence_imaging] [sequence_imaging] 采用序列化拍摄：全景→中景→近景→细节，每张照片标注方位、比例尺与编号 (helpful=2, harmful=0, neutral=0)
- [forensic_indicators] [forensic_indicators] 记录火舌方向、烟熏界线、倒伏痕迹、喷淋头启动状况、配电箱状态等火灾行为与痕迹指标 (helpful=1, harmful=0, neutral=0)
- [annotated_diagrams] [annotated_diagrams] 绘制平面图与剖面图，标注起火区、火势蔓延路径、开口部位、可燃物堆码、消防设施位置与编号；必要时激光测距标注尺寸与北向 (helpful=1, harmful=0, neutral=0)

<!-- ELUCENIA technical documentation · canadian-c-spine-rule · zh · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[条件、来源与许可](https://elucenia.org/zh/tools/canadian-c-spine-rule)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 排除标准：年龄 \< 16 岁、Glasgow \< 15、生命体征异常、创伤超过 48 h、穿透伤、急性瘫痪、已知脊椎疾病/既往颈椎手术、同一损伤复诊或妊娠

`excl`

### 高风险：年龄 ≥ 65 岁

`idade65`

### 高风险：危险机制（坠落 ≥ 0.9 m 或 5 级台阶、头部轴向负荷、高速碰撞、翻车或甩出、机动休闲车辆、自行车碰撞）

`mecanismo`

### 高风险：四肢感觉异常

`parestesia`

### 低风险：简单追尾（无车辆被推向对向车流、大型巴士/卡车撞击、翻车或高速撞击）

`colisao`

### 低风险：在急诊室坐着

`sentado`

### 低风险：伤后曾步行

`deambulou`

### 低风险：延迟出现颈痛

`tardia`

### 低风险：颈椎正中线无压痛

`semdor`

### 能主动向左右各转颈 45° 吗？

`rot`

选填

- `0` — 否
- `1` — 是
- `na` — 尚未检测

### 钝性伤 ≤ 48 h；年龄 ≥ 16 岁、Glasgow 15、生命体征正常，已确认颈痛，或锁骨以上损伤 + 不能步行 + 危险机制的纳入条件？

`contexto`

- `0` — 否
- `1` — 是

## 方法版本

Stiell 2001; Canadian C-Spine Rule

## 已记录的公式

顺序：排除条件→高危因素→存在低危因素→已在临床评估的主动旋转。

## 限制与适用人群

不指导进行颈部运动。未评估颈部旋转时结果不完整。某项标准不存在不等于没有损伤。

## 参考文献

- [Stiell et al. · Canadian C-Spine Rule · 2001年完整论文和标准](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

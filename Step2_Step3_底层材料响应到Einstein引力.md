# Step 2 & 3: 从底物响应到 Einstein 引力，全息与自旋 2 作为推论

## 承接文档：《Step 1: 涌现 Lorentz、等效原理与 Unruh 辐射反作用惯性》

---

## 0. 与 Step 1 的衔接（输入清单）

Step 1 已建立以下结果，本文直接使用（括号内为 Step 1 章节号）：

1. **涌现 Lorentz + 前提 A（单一光锥）**：弦网液体低能极限为相对论性 QFT，所有集体激发共享同一 $c_s$；存在守恒应力-能量张量 $T_{\mu\nu}$ 与四动量 $P^\mu$（Step 1 §1、§3）。
2. **惯性质量的三条等价路径**，均给出 $m_{\text{inertial}} = E_{\text{rest}}/c_s^2$：
   - 路径 (i)：四动量静止系 $00$ 分量，一圈自能 $\Sigma = g^2\Lambda/(4\pi^2)$（Step 1 §3）；
   - 路径 (ii)：加速探测器辐射反作用，$F = -\delta m\, a + (g^2/12\pi c_s^3)\dot a$，协变完成后 $\delta m = U_{\text{field}}/c_s^2 = \Sigma/c_s^2$（Step 1 §5）；
   - 路径 (iii)：$T_{00}$ 源强（Step 1 §7）——其"引力"身份的完整确立依赖本文 §2.4 的普适耦合定理，在 §2.6 闭合。
3. **Unruh–FDT 桥是承重的**：Unruh 温度 $T_U = \hbar a/(2\pi c_s k_B)$ 保证辐射反作用路径在任意加速轨迹上自洽，FDT（$\eta(\omega) = g^2\omega/(4\pi^2 c_s^3)$，温度无关）锁定浴的涨落与反作用匹配（Step 1 §4–§6）。

本文的任务：在此地基上完成 (a) 引力动力学（Einstein 方程作为弦网液体的本构方程）、(b) 等效原理的最终闭合、(c) 自旋 2 与面积律作为推论。

---

## Step 2: 从底物响应到 Einstein 引力

### 2.1 弦网与弯曲背景的耦合

弦段在弯曲背景下的几何长度：

$$
L[\ell] = \int_\ell \sqrt{g_{ij} dx^i dx^j} \approx a_0 \left(1 + \frac{1}{2} h_{ij} t^i t^j\right)
$$

弦网哈密顿量：$H[g] = H_0 + H_{\text{int}}[g]$，其中 $H_{\text{int}}$ 包含弦张力修正和跳变项修正。

### 2.2 自由能泛函

配分函数：$Z[g] = \text{Tr}_{sn}\, e^{-\beta H[g]}$

自由能对度规的泛函展开按 $\sqrt{-g}$ 的完整形式书写（注意 $\sqrt{-g} = 1 + h/2 + O(h^2)$，故"零阶项"同样向各阶 $h$ 贡献，展开按几何结构而非按 $h$ 的幂次分类）：

$$
F[g] = \int d^4x\,\sqrt{-g}\,\rho_0 \;-\; \frac{1}{2}\int d^4x\, h_{\mu\nu}\langle T^{\mu\nu}\rangle \;+\; F^{(2)}[h] \;+\; O(h^3)
$$

- **宇宙学常数项**：$\rho_0 \int d^4x\sqrt{-g}$（真空能，见 §2.6 与待完善内容）
- **源项**：$-\frac{1}{2}\int h_{\mu\nu}\langle T^{\mu\nu}\rangle$（物质应力-能量与度规的耦合；$T_{\mu\nu}$ 的存在性由 Step 1 提供）
- **动力学项** $F^{(2)}[h]$：由对称性唯一确定（§2.3）

### 2.3 对称性约束与 Fierz–Pauli 唯一性（线性）

> **核心假设 B（微分同胚涌现）**：弦网基态只关心弦的拓扑连接，不关心绝对坐标。长波极限下（$L \gg a_0$），坐标重参数化不改变物理，要求 $F[g]$ 在 $g_{\mu\nu}(x) \to g'_{\mu\nu}(x')$ 下不变。**这是本文唯一未从格点证明的输入**（列入待完善内容第一条）。

在线性阶，这要求 $F^{(2)}[h]$ 在规范变换下不变：

$$
h_{\mu\nu} \to h_{\mu\nu} + \partial_\mu \xi_\nu + \partial_\nu \xi_\mu
$$

**Fierz–Pauli 唯一性定理**：在 4 维时空中，满足（1）$h$ 的二阶、（2）至多二阶导数、（3）上述线性规范不变、（4）（涌现）Lorentz 不变的泛函，唯一形式为：

$$
F^{(2)}[h] = -\frac{1}{64\pi G} \int d^4x \left[ (\partial_\lambda h_{\mu\nu})(\partial^\lambda h^{\mu\nu}) - 2(\partial^\lambda h_{\mu\nu})(\partial^\mu h^\nu_{\ \lambda}) + 2(\partial_\mu h)(\partial_\nu h^{\mu\nu}) - (\partial_\mu h)(\partial^\mu h) \right]
$$

即**线性化 Einstein–Hilbert 作用量**。

### 2.4 非线性完成：Deser 自耦合与 Weinberg 普适性

线性理论到完整引力的两步（均为已知定理，非新假设）：

1. **Deser 自耦合重构（1970）**：要求自旋 2 场与其自身应力-能量自洽耦合，逐阶重构在无穷阶求和后唯一给出完整的 Einstein–Hilbert 作用量与非线性微分同胚不变性。等价地，线性规范对称性的一致性形变（consistent deformation）在 4 维无质量自旋 2 情形唯一。
2. **Weinberg soft graviton theorem**：无质量自旋 2 粒子的软极限散射振幅自洽（Lorentz 不变 + 极化张量替换 $\varepsilon_{\mu\nu} \to \partial_\mu \xi_\nu + \partial_\nu \xi_\mu$ 下不变），当且仅当它**以普适强度耦合到所有物质的总守恒 $T_{\mu\nu}$**。

> 第 2 点的直接推论即**等效原理的普适耦合形式**：不存在"只对部分物质耦合"的自洽自旋 2 理论。

### 2.5 Newton 常数与弦网参数

标度关系：

$$
G \sim \frac{\hbar c_s}{T_s}
$$

- $T_s$ 越大（弦越硬）→ $G$ 越小（引力越弱）
- 精确系数由弦网弹性模量 $K$ 和弦密度 $\rho_s$ 决定：$1/G \propto K \rho_s^2 c_s^2$

### 2.6 Einstein 方程作为本构方程 + 等效原理的最终闭合

变分完整自由能（含宇宙学常数项，与 §2.2 一致）：

$$
G_{\mu\nu} + \Lambda g_{\mu\nu} = 8\pi G\, T_{\mu\nu}, \qquad \Lambda \sim \frac{8\pi G \rho_0}{c_s^4}
$$

（$\Lambda$ 的保留与 $F^{(0)}$ 一致；这使宇宙学常数问题在场方程层面直接显形：弦网真空能 $\rho_0$ 天然在截断标度，远大于观测值——见待完善内容。）

**等效原理的最终闭合**——Step 1 的三条质量路径在此汇齐：

| 质量 | 路径 | 数值 |
|------|------|------|
| $m_{\text{inertial}}$ | (i) 四动量 $P^\mu$ 静止系 $00$ 分量（Step 1 §3） | $E_{\text{rest}}/c_s^2$ |
| $m_{\text{inertial}}$ | (ii) 加速探测器辐射反作用系数，$\delta m = U_{\text{field}}/c_s^2$（Step 1 §5） | $E_{\text{rest}}/c_s^2$ |
| $m_{\text{grav}}$ | (iii) $T_{00}$ 源强；由 §2.4-2，自旋 2 耦合普适，无任何物质例外 | $E_{\text{rest}}/c_s^2$ |

$$
\boxed{\;m_{\text{inertial}} = m_{\text{grav}} = \frac{E_{\text{rest}}}{c_s^2}\;}
$$

> **核心定理**：在弦网液体的有效场论中，等效原理是 涌现 Lorentz（前提 A）+ 微分同胚涌现（假设 B）+ 自旋 2 耦合自洽性（Weinberg 定理）的推论。其全部非平凡内容被精确隔离在前提 A 与假设 B 中。Unruh–FDT 桥（Step 1 §4–§6）保证惯性在任意加速观察者参考系中表现一致——路径 (ii) 的合法性正是由它担保。

**类比**：
- Navier–Stokes = 流体分子运动论的本构方程
- Einstein = 时空介质（弦网液体）的宏观本构方程

---

## Step 3: 全息与自旋 2 作为推论

### 3.1 Spin-2 作为推论

从 Step 2 的 $F^{(2)}[h]$，变分得到运动方程：

$$
\Box \bar{h}_{\mu\nu} = -\frac{16\pi G}{c_s^4} \delta T_{\mu\nu}
$$

**自由传播**（无源）：$\Box \bar{h}_{\mu\nu} = 0$

**规范条件**：$\partial^\mu \bar{h}_{\mu\nu} = 0$（横向，4 个约束），$\bar{h}^\mu_{\ \mu} = 0$（无迹，1 个约束），剩余规范自由度（保持无迹的谐和 $\xi_\mu$，3 个函数）。

**自由度计数**：对称张量 10 分量 − 横向 4 − 无迹 1 − 剩余规范 3 = **2 个物理偏振**

**偏振张量**：

$$
\varepsilon_{ij}^{(+)} : h_{xx} = -h_{yy} = \frac{1}{\sqrt{2}}, \qquad \varepsilon_{ij}^{(\times)} : h_{xy} = h_{yx} = \frac{1}{\sqrt{2}}
$$

→ 标准自旋 2 的 + 和 × 偏振。

> **反馈关系（注意方向）**：正是本节的"无质量自旋 2 + 2 偏振"结论，反过来许可了 §2.4 的 Weinberg 定理适用——而 Weinberg 定理闭合了 §2.6 的等效原理。自旋 2 不只是推论，也是 EP 论证链的必要环节。

### 3.2 全息（面积律）作为推论

**弦网基态纠缠熵**（拓扑序面积律）：

$$
S(\rho_\Sigma) = \alpha \cdot \text{Area}(\Sigma) - \gamma + O(1/L)
$$

物理来源：纠缠由穿过曲面 $\Sigma$ 的弦贡献，闭合在内部的弦不产生纠缠。

**与 Bekenstein–Hawking 熵对应**：

$$
S_{BH} = \frac{k_B \cdot \text{Area}(\Sigma)}{4 l_P^2} = \frac{k_B c_s^3 \cdot \text{Area}(\Sigma)}{4 G \hbar}
$$

令 $S_{sn} = S_{BH}$：

$$
\alpha = \frac{k_B c_s^3}{4 G \hbar} = \frac{k_B c_s^2\, T_s}{4\hbar^2} \;\propto\; T_s
$$

物理图像自洽：弦越硬 → $G$ 越小 → $l_P^2 = G\hbar/c_s^3$ 越小 → 单位面积的熵越大。与 §2.5 的 $G \sim \hbar c_s / T_s$ 自洽。

---

## 五个问题的回答

| 问题 | 回答 |
|------|------|
| **底层自由度是什么** | 弦构型（闭合弦 + 弦末端费米子），满足融合规则 |
| **Hamiltonian 是什么** | $H = H_{\text{fusion}} + H_{\text{string}} + H_{\text{end}}$，非相对论 |
| **Lorentz 为什么出现** | Wen 定理：弦网低能谱线性 → 涌现洛伦兹协变；外加前提 A（单一光锥）保证所有激发共享同一 $c_s$（Step 1） |
| **惯性为什么存在** | 三条等价路径：静能 $E_{\text{rest}}/c_s^2$、加速探测器辐射反作用 $\delta m = U_{\text{field}}/c_s^2$、$T_{00}$ 源强（Step 1）；Unruh–FDT 桥保证其参考系无关性 |
| **Spin-2 为什么出现** | 坐标重参数化不变性（假设 B）→ 对称张量场 → d=4 下 TT 规范剩 2 个偏振（§3.1） |
| **Einstein 方程为什么出现** | 弦网自由能 + 长波极限 + 微分同胚不变性（假设 B）→ Fierz–Pauli 唯一（线性）→ Deser/Weinberg 自洽（非线性 + 普适耦合）（§2.3–2.6） |
| **等效原理为什么成立** | 涌现 Lorentz ⇒ 惯性 = $E_{\text{rest}}/c_s^2$（两条独立路径互验）；Weinberg 普适耦合 ⇒ 引力质量为同一量。归约到前提 A + 假设 B（§2.6） |

---

## 待完善内容

| 已证明（EFT 层面 + 标准定理） | 仍需格点严格化 |
|-----------|---------------|
| Fierz–Pauli → Deser/Weinberg → EH + 普适耦合（标准定理链） | **假设 B：从格点弦网第一性原理证明长波微分同胚对称性**（本文唯一核心未证输入） |
| EP：三条质量路径汇于 $E_{\text{rest}}/c_s^2$（归约到前提 A + 假设 B） | **前提 A：所有低能集体激发共享同一 $c_s$**（多度规问题；引力模与物质模速度相等的具体论证） |
| 自旋 2 偏振计数（10 − 4 − 1 − 3 = 2） | 格点引力子产生算符的显式构造 |
| 面积律与 Bekenstein–Hawking 对应（$\alpha \propto T_s$） | Einstein 方程作为本构方程的粗粒化严格推导 |
| $G \sim \hbar c_s/T_s$ 标度关系 | $1/G \propto K\rho_s^2 c_s^2$ 精确系数的格点计算 |
| 宇宙学常数项在场方程中显形（$G_{\mu\nu}+\Lambda g_{\mu\nu}=8\pi GT_{\mu\nu}$） | 宇宙学常数问题（$\rho_0$ 在截断标度 vs 观测值） |
| — | 黑洞信息悖论（获得新表述但未解决） |

> Step 1 侧的待完善事项（辐射反作用展开的相对论全阶形式、协变完成的显式格点构造、匀加速标量荷辐射的逐模验证等）见 Step 1 文档 §10。

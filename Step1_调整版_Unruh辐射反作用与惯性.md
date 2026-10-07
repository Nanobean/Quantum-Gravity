# Step 1: 涌现 Lorentz、等效原理与 Unruh 辐射反作用惯性

## 从弦网液体到等效原理的显式推导（含加速探测器辐射反作用计算）

---

## 0. 总览：惯性质量的三条路径

本文在弦网液体的低能有效场论中，从三条独立路径计算同一个准粒子的惯性质量：

| 路径 | 物理对象 | 所在节 |
|------|---------|--------|
| (i) 静能路径 | 四动量 $P^\mu$ 的静止系 $00$ 分量；一圈自能 | §3 |
| (ii) 辐射反作用路径 | 加速探测器自力的反作用系数（Jaekel–Reynaud 路线） | §5 |
| (iii) 引力源路径 | 应力-能量张量 $T_{00}$ 的源强 | §7 |

三条路径给出**同一个** $E_{\text{rest}}/c_s^2$——这是等效原理在本框架内的完整形态。其中路径 (ii) 把 Unruh 效应与惯性直接联系起来：惯性是加速探测器与 Unruh 浴（真空涨落在加速系中的热形态）相互作用的**反作用部分**，而浴的涨落部分由同一耦合经 FDT 给出。

中间计算采用自然单位 $\hbar = c_s = 1$，关键结果恢复单位后给出。

---

## 1. 物理设定与模型

弦网液体的低能有效场论：在长波极限下，弦密度涨落 $\phi(x,t)$ 的声学支满足线性色散

$$
\omega_k = c_s |k|
$$

其中 $c_s$ 是弦网声速（涌现的"光速"）。有效作用量为无质量标量场：

$$
S = \frac{1}{2} \int dt\, d^3x \left[ (\partial_t \phi)^2 - c_s^2 (\nabla \phi)^2 \right]
$$

**关键事实**：母理论是非相对论的（有优选系——弦网静止系），但低能下 Lorentz 对称性涌现，且涌现的"光速"就是 $c_s$。这是 Wen 的已有定理。

**前提 A（单一光锥）**：弦网液体的所有低能集体激发——声学标量模、规范玻色子、弦末端费米子、以及自旋 2 引力模——在长波极限下共享同一极限速度 $c_s$。在格点模型中不同集体激发一般速度不同（多度规风险），故此非自动成立；其格点证明列入待完善内容（§10）。本文全部结论以前提 A 为前提。

准粒子（弦末端费米子）与声学场单极耦合：

$$
H_{\text{int}} = g \int d^3x\; \psi^\dagger\psi\, \phi
$$

点粒子极限下 $\psi^\dagger\psi \to \delta^3(\mathbf{x} - \mathbf{z}(t))$，$\mathbf{z}(t)$ 为准粒子轨迹。

---

## 2. Minkowski 模式展开

$$
\phi(t, \mathbf{x}) = \int \frac{d^3k}{(2\pi)^3} \frac{1}{\sqrt{2\omega_k}} \left[ a_k e^{-i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} + a_k^\dagger e^{+i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} \right]
$$

$$
[a_k, a_{k'}^\dagger] = (2\pi)^3 \delta^3(\mathbf{k} - \mathbf{k}')
$$

Minkowski 真空 $|0\rangle_M$（即弦网基态的低能描述）由 $a_k |0\rangle_M = 0$ 定义。

---

## 3. 路径一：四动量定义与一圈自能

### 3.1 定义

涌现 Lorentz 对称性（§1 + 前提 A）保证低能理论是相对论性量子场论：能量与动量组成四矢量 $P^\mu = (E/c_s, \mathbf{p})$。对静止束缚态（准粒子 + 其自能云），惯性质量定义为

$$
m_{\text{inertial}} \equiv \frac{E_{\text{rest}}}{c_s^2}
$$

这是恒等式而非机制：洛伦兹协变性保证四矢量各分量按同一规则变换，静止系 $00$ 分量就是阻碍加速的量。

### 3.2 一圈自能

静能由弦网微观参数唯一确定：$E_{\text{rest}} = m_0 c_s^2 + \Sigma + \cdots$。自能修正由 $H_{\text{int}}$ 的二阶微扰给出（矩阵元 $1/\sqrt{2\omega_k}$，能量分母 $\sim \omega_k$，自然单位）：

$$
\Sigma = g^2 \int^{\Lambda} \frac{d^3k}{(2\pi)^3} \frac{1}{2\omega_k^2} = \frac{g^2 \Lambda}{4\pi^2}
$$

（$\Lambda \sim 1/a_0$ 为晶格截断，$a_0$ 为晶格常数。）恢复单位：

$$
\delta m = \frac{\Sigma}{c_s^2} \sim \frac{g^2}{4\pi^2\, c_s^2\, a_0}
$$

即原方案积分 $g^2\int^\Lambda d^3k/\omega_k^2$ 的正确物理身份：**一圈自能（质量重正化）**。温度无关、与加速度无关。

---

## 4. Unruh 效应

**Rindler 坐标**（相对弦网背景匀加速 $a$ 的观察者）：

$$
c_s t = \rho \sinh\!\left(\frac{a\xi}{c_s}\right), \qquad x = \rho \cosh\!\left(\frac{a\xi}{c_s}\right), \qquad ds^2 = -\left(\frac{a\rho}{c_s}\right)^2 d\xi^2 + d\rho^2 + dy^2 + dz^2
$$

**Bogoliubov 变换**（复 $\xi$ 平面解析延拓 $i\pi c_s/a$）：

$$
\frac{|\beta_k|^2}{|\alpha_k|^2} = e^{-2\pi\Omega c_s / a}
$$

由 $|\alpha|^2 - |\beta|^2 = 1$：

$$
|\beta|^2 = \frac{1}{e^{2\pi\Omega c_s / a} - 1} \;\;\Rightarrow\;\; \beta_R = \frac{2\pi c_s}{a\hbar} \;\;\Rightarrow\;\; T_{\text{Unruh}} = \frac{\hbar a}{2\pi c_s k_B}
$$

（严格处理需有限体积或探测器响应函数以处理连续谱归一化；结论不变。）

> **本节结果的双重身份**：(a) 它是涌现时空量子自洽性的判据——加速观察者必须看到精确热浴，涌现 Lorentz 才是量子层面真实的对称性；(b) 它是下一节辐射反作用计算的工作介质——加速准粒子的自力涨落部分正是与这个 $T_U$ 热浴的交换。

---

## 5. 路径二：加速探测器的辐射反作用（Jaekel–Reynaud 路线）

本节是 Unruh 效应与惯性质量之间的直接计算。思路：准粒子是声学场的点单极源；它在任意轨迹上运动时激发自场；自场反作用于源。自力的**对称（反作用）部分**正比于加速度——其系数就是惯性质量；**反对称（辐射）部分**描述与 Unruh 浴的量子交换——由 FDT 锁定在 $T_U$。

### 5.1 模型：轨迹上的点单极源

准粒子沿 prescribed 轨迹 $\mathbf{z}(t)$ 运动，场方程（自然单位）：

$$
\Box\, \phi = -g\, \delta^3(\mathbf{x} - \mathbf{z}(t)), \qquad \Box = -\partial_t^2 + \nabla^2
$$

推迟解为标量 Liénard–Wiechert 势。匀速 $\mathbf{v}$（$\beta = v/c_s$，恢复 $c_s$）时：

$$
\phi(\mathbf{x}, t) = \frac{g}{4\pi}\, \frac{1}{\sqrt{(z - vt)^2 + (1 - \beta^2)(x^2 + y^2)}}
$$

### 5.2 自力的对称化分解

场分解为真空涨落与自场：$\phi = \phi_0 + \phi_{\text{sc}}$。平均自力（外场已减除）：

$$
F_i(t) = g\, \langle \partial_i \phi_{\text{sc}}(\mathbf{z}(t), t) \rangle
$$

将自场按时间反演分解：

$$
\phi_{\text{sc}} = \underbrace{\tfrac{1}{2}(\phi_{\text{ret}} + \phi_{\text{adv}})}_{\text{对称（反作用）}\;\to\;\text{惯性}} + \underbrace{\tfrac{1}{2}(\phi_{\text{ret}} - \phi_{\text{adv}})}_{\text{反对称（辐射）}\;\to\;\text{Unruh 量子交换}}
$$

### 5.3 非相对论轨迹展开

对推迟自场在粒子位置做标准 Lorentz 导数展开（$|v| \ll c_s$），得：

$$
\boxed{\;F(t) = -\delta m\, a(t) + \frac{g^2}{12\pi c_s^3}\, \dot{a}(t) + O(\ddot{a})\;}
$$

- **第一项**：正比于加速度，系数即惯性质量的场贡献；
- **第二项**：标量版 Abraham–Lorentz 辐射反作用，特征时间 $\tau_0 = g^2/(12\pi m c_s^3)$，截断无关；
- 对匀加速轨迹 $\dot a = 0$，辐射反作用项消失，**剩下纯惯性响应**——这正是质量可从匀加速实验提取的原因。

### 5.4 2/3 因子与协变完成：$\delta m = U_{\text{field}}/c_s^2$

惯性项系数的裸计算（各向同性截断）经由场动量进行：匀速运动单极源的场动量与场能（直接积分，本文已数值核验，$\beta \to 0$ 极限精确）：

$$
\mathbf{p}_{\text{field}} = \frac{2}{3}\, \frac{U_{\text{field}}}{c_s^2}\, \mathbf{v}, \qquad U_{\text{field}} = \frac{1}{2}\int d^3x\, c_s^2 (\nabla\phi)^2 = \frac{c_s^2 g^2 \Lambda}{4\pi^2}
$$

因子 $2/3$ 是经典电子论 $4/3$ 问题的标量版（电磁情形为 $4/3$，源于场单独的能动量不构成四矢量）。解决途径相同：准粒子不是裸点荷，而是**完整相对论性束缚态**——弦网内部结合应力（Poincaré 应力的涌现对应物）贡献其余 $1/3$，使总能量-动量恢复四矢量性。涌现 Lorentz 对称性（§1）正是这一完成的保证：

$$
\delta m = \frac{U_{\text{field}}}{c_s^2} = \frac{g^2 \Lambda}{4\pi^2} \quad (\hbar = c_s = 1)
$$

与 §3.2 对照：$U_{\text{field}} = \frac{1}{2}\int c_s^2 k^2 |\phi_k|^2 = g^2\int \frac{d^3k}{(2\pi)^3}\frac{1}{2\omega_k^2}\big|_{\text{同截断}} = \Sigma$。**经典场能与一圈自能是同一个积分**——因此：

$$
\boxed{\;\delta m_{\text{辐射反作用}} = \frac{U_{\text{field}}}{c_s^2} = \frac{\Sigma}{c_s^2} = \delta m_{\text{静能}}\;}
$$

这就是 Jaekel–Reynaud 一致性结果的声学版：**由辐射反作用测得的惯性，等于由哈密顿量自能算得的质量**。两条路径不是两个机制，而是同一耦合 $g$ 的自洽性两端——动力学（自力）与运动学（能量）给出同一惯性。

### 5.5 匀加速情形：与 Unruh 浴的平衡

匀加速轨迹（双曲线运动）下：

1. **惯性项**：维持加速所需外力为 $F_{\text{ext}} = (m_0 + \delta m)\, a$，其中 $\delta m$ 即上式；
2. **剩余辐射项**：标量单极的四维自力为 $F^\mu = \frac{g^2}{12\pi c_s^3}\left(\dot a^\mu + \frac{a_\nu a^\nu}{c_s^2} u^\mu\right)$（标量 ALD 方程；注意与电磁情形的符号差——电磁为减号，匀加速下严格为零；标量为加号）。双曲线运动下 $\dot a^\mu = (a_\nu a^\nu/c_s^2) u^\mu$，故标量情形存在非零剩余项 $\propto a^2 u^\mu$：匀加速标量荷**确实辐射**。
3. **Rindler 系诠释**：在随动 Rindler 系中探测器静止，浸在 $T_U = \hbar a/(2\pi c_s k_B)$ 的 Unruh 浴中。探测器向浴发射 Rindler 量子的速率与从浴吸收的速率在热平衡下精确相抵（§4 的玻色分布保证）；实验室系看到的"匀加速标量荷辐射"与 Rindler 系看到的"与 Unruh 浴的净交换"是同一物理的两种描述。剩余辐射项的涨落关联由 §6 的 FDT 在 $T = T_U$ 处锁定。

于是加速准粒子的完整运动方程为：

$$
m_0\, \dot v = F_{\text{ext}} \underbrace{-\; \delta m\, a}_{\text{浴的反作用（惯性）}} \underbrace{+\; F_{\text{rad}}}_{\text{Unruh 净交换}} \underbrace{+\; F_{\text{fluc}}(T_U)}_{\text{浴的涨落}}
$$

> **Unruh–惯性联系的精确形态**：惯性不是 Unruh 浴的"拖曳"（不存在，见 §6），而是加速探测器与真空/Unruh 涨落相互作用的**反作用部分**；Unruh 效应保证这一反作用在所有加速系中自洽，FDT 保证反作用与涨落匹配。原方案的方向在此意义上被复活——只是把"静止系粘滞摩擦"换成了"加速轨迹的辐射反作用"。

### 5.6 一致性的物理含义

| | 路径 (i) 静能 | 路径 (ii) 辐射反作用 | 路径 (iii) 引力源（§7） |
|---|---|---|---|
| 计算对象 | 哈密顿量二阶微扰 | 自力反作用系数 | $T_{00}$ 源强 |
| 结果 | $\Sigma/c_s^2$ | $U_{\text{field}}/c_s^2$ | $E_{\text{rest}}/c_s^2$ |

三者是同一个积分、同一个 $E_{\text{rest}}$。

---

## 6. 涨落-耗散定理：浴的合格性检验

**随机力关联**（温度 $\beta$ 的声学浴）：

$$
C_F(t) = g^2 \langle \{ \phi(0, t), \phi(0, 0) \} \rangle = g^2 \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \coth\!\left(\frac{\beta\hbar\omega_k}{2}\right) \cos(\omega_k t)
$$

**耗散核**（线性响应，对易子给出，显式结果）：

$$
\eta(\omega) = \frac{g^2}{2} \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \left[ \delta(\omega - \omega_k) + \delta(\omega + \omega_k) \right] = \frac{g^2}{4\pi^2}\, \frac{\omega}{c_s^3}
$$

**FDT**：$C_F(\omega) = 2\eta(\omega)\, \hbar \coth(\beta\hbar\omega/2)$ 成立（EFT 层面）。三个明确记录的性质：

- $\eta$ **与温度无关**（耗散由对易子决定，$\coth$ 只进噪声关联）——FDT 的内容正在于此；
- $\eta(\omega) \propto \omega$，**$\eta(0) = 0$**：该浴不存在常数 Markov 摩擦系数——不存在可供定义为质量的静态拖曳 $-\eta V$。这从反面确认了质量只能来自 §3 的静能与 §5 的辐射反作用；
- 任何 $\propto V$ 的拖曳都相对弦网静止系，与涌现 Lorentz 不变性冲突：洛伦兹不变真空中匀速粒子不受拖曳。

对加速探测器，上式取 $T = T_U$ 即给出 §5.5 涨落力 $F_{\text{fluc}}$ 的关联——反作用与涨落在同一耦合 $g$ 下匹配，浴合格。高温经典极限下 Einstein 关系 $D = k_B T/\eta$ 成立。

---

## 7. 等效原理：三条路径汇于一点

### 7.1 引力质量

同一准粒子作为弦网应力-能量的源，静止时：

$$
T_{00} = E_{\text{rest}}\, \delta^3(\mathbf{x}) \quad\Rightarrow\quad m_{\text{grav}} = \frac{E_{\text{rest}}}{c_s^2}
$$

### 7.2 恒等式

| 质量 | 路径 | 数值 |
|------|------|------|
| $m_{\text{inertial}}$ | (i) 四动量静止系 $00$ 分量；(ii) 辐射反作用系数 | $E_{\text{rest}}/c_s^2$ |
| $m_{\text{grav}}$ | (iii) $T_{00}$ 源强 | $E_{\text{rest}}/c_s^2$ |

$$
\frac{m_{\text{inertial}}}{m_{\text{grav}}} = 1
$$

三者不是三个碰巧同标度的效应，而是同一个量 $E_{\text{rest}}/c_s^2$ 的三个读法。

### 7.3 前提的精确清单

该恒等式依赖且仅依赖：

1. **前提 A（单一光锥）**：所有低能场共享同一 $c_s$；
2. **引力场以普适强度耦合到总 $T_{\mu\nu}$**：在 Step 2 给出无质量自旋 2 场后，由 Weinberg 自洽耦合定理（soft graviton theorem）完成——无质量自旋 2 场的任何自洽耦合必然普适地耦合到守恒总应力-能量张量上。等效原理的最终闭合在 Step 2。

### 7.4 与标准物理的对比

- **标准物理**：GR 中普适耦合是输入假设，实验验证到 $10^{-15}$（MICROSCOPE）。
- **弦网框架**：普适耦合归约为两个结构性命题——(i) 单一光锥（前提 A）；(ii) 弦网拓扑序的长波微分同胚不变性（Step 2 的输入）。等效原理不是独立假设。

> **核心陈述**：在弦网液体的有效场论中，等效原理是涌现 Lorentz 对称性 + 自旋 2 耦合自洽性的推论。惯性同时有三个等价表现——静能、辐射反作用、引力源强——而 Unruh 效应与 FDT 保证第二种表现在任意加速轨迹上自洽。

---

## 8. 结构总结

```
弦网基态 |Ψ₀⟩（非相对论母理论）
        ↓
低能有效场论：声学场 φ，ω = c_s|k|（Wen 定理）
        ↓
前提 A：单一光锥（所有低能激发共享 c_s）
        ↓
相对论性 QFT → P^μ 四矢量、守恒 T_μν
        ↓
惯性质量的三条等价路径：
  (i)  静能：      m = E_rest/c_s²，Σ = g²Λ/(4π²)（一圈自能）
  (ii) 辐射反作用： F = -δm a + (g²/12πc_s³)ȧ，
                    协变完成（2/3 → 1）后 δm = U_field/c_s² = Σ/c_s²
  (iii) 引力源：    T_00 = E_rest δ³(x)
        ↓
Unruh（T = ħa/2πc_s k_B）+ FDT：
  保证路径 (ii) 在任意加速轨迹上自洽
  （反作用 ↔ T_U 涨落，同一 g）
        ↓
〔Step 2：自旋 2 + Weinberg 普适耦合 → EP 最终闭合〕
        ↓
m_inertial = m_grav（同一量的三个读法）
```

---

## 9. 与评论者路线的对应

评论者要求的：*Emergent Lorentz–Unruh–FDT bridge*

| 要求 | 完成状态 | 功能 |
|------|---------|------|
| Lorentz 涌现 | ✅ Wen 定理 + 前提 A（单一光锥） | 承重：一切的前提 |
| Unruh | ✅ Bogoliubov 显式算出 $T = \hbar a/(2\pi c_s k_B)$；§5.5 给出 Rindler 系平衡诠释 | **双重功能**：自洽性判据 + 辐射反作用的工作介质 |
| FDT | ✅ 显式验证（含 $\eta(\omega) = g^2\omega/(4\pi^2 c_s^3)$）；锁定 $T_U$ 处涨落 | 反作用与涨落的匹配条件 |
| Bridge | ✅ §5：加速探测器辐射反作用给出 $\delta m = \Sigma/c_s^2$，与静能路径、引力源路径三方一致 | **桥现在是承重的**：Unruh 浴的反作用即惯性 |

---

## 10. 待完善内容

| 已证明（EFT 层面） | 仍待证明 / 已知局限 |
|--------|---------------------|
| Unruh 效应（Bogoliubov，含 $T_U$） | 前提 A：所有低能激发共享 $c_s$ 的格点证明（多度规问题） |
| 辐射反作用展开 $F = -\delta m\, a + \tau_0 m\, \dot a$（非相对论阶） | 展开的相对论全阶形式；$\tau_0$ 的 $O(1)$ 系数依赖正规化约定 |
| $\delta m = U_{\text{field}}/c_s^2 = \Sigma/c_s^2$（三方一致性） | 协变完成的显式构造（弦网内部结合应力的格点计算；本文以涌现 Lorentz 论证其必然性，类比 Poincaré 应力） |
| 标量 ALD 剩余项的 Rindler 诠释（定性） | 匀加速标量荷辐射的探测器层面显式验证（发射/吸收速率逐模匹配） |
| FDT（含 $\eta \propto \omega$、$\eta(0)=0$、$T$ 无关性） | 从格点弦网第一性原理证明微分同胚对称性（Step 2 的输入） |
| 自能标度 $\delta m \sim g^2/(c_s^2 a_0)$ | 自能 $O(1)$ 系数的正规化方案固定；Einstein 方程粗粒化（Step 2）；宇宙学常数问题 |

> **与原方案的关系（存档注记）**：原 "Unruh → FDT → 拖曳 → $m \equiv F_{\text{drift}}/a$" 路线被 §6 的显式计算排除（$\eta$ 温度无关、$\eta(0)=0$、洛伦兹破缺、$\eta\tau_{\text{relax}}$ 循环定义）。本文 §5 表明 Unruh–惯性联系的正确形态是**加速轨迹的辐射反作用**：浴的反作用（而非粘滞拖曳）提供惯性，且与静能路径严格一致。Unruh 效应由此从"自洽性检验"恢复为推导链的承重环节——但以动力学上唯一自洽的方式。

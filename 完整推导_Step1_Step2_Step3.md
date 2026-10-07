# 弦网引力三步闭环推导

## Step 1: Emergent Lorentz–Unruh–FDT Bridge
## Step 2: From Substrate Response to Einstein Gravity
## Step 3: Holography and Spin-2 as Consequences

---

## 总纲

本推导按知乎@夏草建议的三步路线，将弦网凝聚、Le Sage 屏蔽机制、Verlinde 熵力和等效原理统一为可计算的物理框架。

| 步骤 | 目标 | 核心结果 |
|------|------|---------|
| Step 1 | Lorentz–Unruh–FDT 桥梁 | Unruh温度从弦网谱显式算出，EP是恒等式 |
| Step 2 | 底物响应到 Einstein 引力 | Einstein方程作为弦网液体的宏观本构方程 |
| Step 3 | 全息与自旋2作为推论 | 偏振计数→自旋2；面积律→Bekenstein-Hawking熵 |

---

## Step 1: Emergent Lorentz–Unruh–FDT Bridge

### 1.1 物理设定

弦网液体的低能有效场论：长波极限下，弦密度涨落 $\phi(x,t)$ 的声学支满足线性色散

$$
\omega_k = c_s |k|
$$

有效作用量（无质量标量场，$c$ 替换为声速 $c_s$）：

$$
S = \frac{1}{2} \int dt d^3x \left[ (\partial_t \phi)^2 - c_s^2 (\nabla \phi)^2 \right]
$$

**关键事实**：母理论是非相对论的（有优选系——弦网静止系），但低能下 Lorentz 对称性涌现。这是 Wen 的已有定理。

### 1.2 Unruh 效应的显式推导

**Minkowski 模式展开**：

$$
\phi(t, \mathbf{x}) = \int \frac{d^3k}{(2\pi)^3} \frac{1}{\sqrt{2\omega_k}} \left[ a_k e^{-i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} + a_k^\dagger e^{+i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} \right]
$$

**Rindler 坐标**（加速观察者，加速度 $a$）：

$$
c_s t = \rho \sinh\!\left(\frac{a\xi}{c_s}\right), \quad x = \rho \cosh\!\left(\frac{a\xi}{c_s}\right)
$$

**Bogoliubov 变换**（解析延拓 $i\pi c_s/a$）：

$$
\frac{|\beta_k|^2}{|\alpha_k|^2} = e^{-2\pi\Omega c_s / a}
$$

**Unruh 温度**：

$$
T_{\text{Unruh}} = \frac{\hbar a}{2\pi c_s k_B}
$$

### 1.3 涨落-耗散定理（FDT）

弦末端准粒子与弦网声学涨落耦合：$H_{\text{int}} = g \psi^\dagger\psi \phi(0,t)$

**随机力关联**：

$$
C_F(t) = g^2 \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \coth\!\left(\frac{\beta\hbar\omega_k}{2}\right) \cos(\omega_k t)
$$

**耗散核**：

$$
\eta(\omega) = \frac{g^2}{2} \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \left[ \delta(\omega - \omega_k) + \delta(\omega + \omega_k) \right]
$$

**FDT 验证**：$C_F(\omega) = 2\eta(\omega) \hbar \coth(\beta\hbar\omega/2)$，严格成立。

### 1.4 质量定义与等效原理

**质量定义**：

$$
m \equiv \frac{F_{\text{drift}}}{a} = g^2 \int^{\Lambda} \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k^2} \sim \frac{g^2}{c_s^2 a_0}
$$

**等效原理**：

| 质量类型 | 来源 | 标度 |
|---------|------|------|
| $m_{\text{inertial}}$ | 拖曳弦网涨落的阻抗 | $\propto g^2/(c_s^2 a_0)$ |
| $m_{\text{grav}}$ | 作为应力-能量张量的源 | $\propto g^2/(c_s^2 a_0)$ |

$$
\frac{m_{\text{inertial}}}{m_{\text{grav}}} = 1 \quad \text{（同一耦合 } g \text{ 的恒等式）}
$$

---

## Step 2: From Substrate Response to Einstein Gravity

### 2.1 弦网与弯曲背景的耦合

弦段在弯曲背景下的几何长度：

$$
L[\ell] = \int_\ell \sqrt{g_{ij} dx^i dx^j} \approx a_0 \left(1 + \frac{1}{2} h_{ij} t^i t^j\right)
$$

弦网哈密顿量：$H[g] = H_0 + H_{\text{int}}[g]$，其中 $H_{\text{int}}$ 包含弦张力修正和跳变项修正。

### 2.2 自由能泛函

配分函数：$Z[g] = \text{Tr}_{sn} e^{-\beta H[g]}$

自由能展开：$F[g] = F^{(0)} + F^{(1)}[h] + F^{(2)}[h] + O(h^3)$

- **零阶**（宇宙学常数）：$F^{(0)} = \rho_0 \int d^4x \sqrt{-g}$
- **一阶**（应力-能量源）：$F^{(1)} = -(1/2) \int h_{\mu\nu} \langle T^{\mu\nu} \rangle$
- **二阶**（动力学）：由对称性唯一确定

### 2.3 对称性约束与唯一性

弦网基态只关心弦的拓扑连接，不关心绝对坐标。长波极限下（$L \gg a_0$），坐标重参数化不改变物理，要求 $F[g]$ 在 $g_{\mu\nu}(x) \to g'_{\mu\nu}(x')$ 下不变。

在线性阶，这要求 $F^{(2)}[h]$ 在规范变换下不变：

$$
h_{\mu\nu} \to h_{\mu\nu} + \partial_\mu \xi_\nu + \partial_\nu \xi_\mu
$$

**唯一性定理**：在4维时空中，满足（1）$h$ 的二阶、（2）至多二阶导数、（3）规范不变、（4）洛伦兹不变的泛函，唯一形式为：

$$
F^{(2)}[h] = -\frac{1}{64\pi G} \int d^4x \left[ (\partial_\lambda h_{\mu\nu})(\partial^\lambda h^{\mu\nu}) - 2(\partial^\lambda h_{\mu\nu})(\partial^\mu h^\nu_\lambda) + 2(\partial_\mu h)(\partial_\nu h^{\mu\nu}) - (\partial_\mu h)(\partial^\mu h) \right]
$$

这正是**线性化 Einstein-Hilbert 作用量**。

### 2.4 Newton 常数与弦网参数

标度关系：

$$
G \sim \frac{\hbar c_s}{T_s}
$$

- $T_s$ 越大（弦越硬）→ $G$ 越小（引力越弱）
- 精确系数由弦网弹性模量 $K$ 和弦密度 $\rho_s$ 决定：$1/G \propto K \rho_s^2 c_s^2$

### 2.5 Einstein 方程作为本构方程

变分 $F^{(0)} + F^{(1)} + F^{(2)}$ 得：

$$
G_{\mu\nu} = 8\pi G T_{\mu\nu}
$$

**类比**：
- Navier-Stokes = 流体分子运动论的本构方程
- Einstein = 时空介质（弦网液体）的宏观本构方程

---

## Step 3: Holography and Spin-2 as Consequences

### 3.1 Spin-2 作为推论

从 Step 2 的 $F^{(2)}[h]$，变分得到运动方程：

$$
\Box \bar{h}_{\mu\nu} = -\frac{16\pi G}{c_s^4} \delta T_{\mu\nu}
$$

**自由传播**（无源）：$\Box \bar{h}_{\mu\nu} = 0$

**规范条件**：$\partial^\mu \bar{h}_{\mu\nu} = 0$（横向），$\bar{h}^\mu_\mu = 0$（无迹）

**自由度计数**：对称张量10分量 - 横向4 - 无迹1 - 冗余3 = **2个物理偏振**

**偏振张量**：

$$
\varepsilon_{ij}^{(+)} : h_{xx} = -h_{yy} = \frac{1}{\sqrt{2}}, \quad \varepsilon_{ij}^{(\times)} : h_{xy} = h_{yx} = \frac{1}{\sqrt{2}}
$$

→ 标准自旋2的 + 和 × 偏振。

### 3.2 全息（面积律）作为推论

**弦网基态纠缠熵**（拓扑序面积律）：

$$
S(\rho_\Sigma) = \alpha \cdot \text{Area}(\Sigma) - \gamma + O(1/L)
$$

物理来源：纠缠由穿过曲面 $\Sigma$ 的弦贡献，闭合在内部的弦不产生纠缠。

**与 Bekenstein-Hawking 熵对应**：

$$
S_{BH} = \frac{k_B \cdot \text{Area}(\Sigma)}{4 l_P^2} = \frac{k_B c_s^3 \cdot \text{Area}(\Sigma)}{4 G \hbar}
$$

令 $S_{sn} = S_{BH}$：

$$
\alpha = \frac{k_B c_s^3}{4 G \hbar} \sim \frac{k_B c_s^2}{T_s}
$$

与 Step 2 的 $G \sim \hbar c_s / T_s$ 自洽。

---

## 五个问题的回答

| 问题 | 回答 |
|------|------|
| **底层自由度是什么** | 弦构型（闭合弦+弦末端费米子），满足融合规则 |
| **Hamiltonian是什么** | $H = H_{\text{fusion}} + H_{\text{string}} + H_{\text{end}}$，非相对论 |
| **Lorentz为什么出现** | Wen定理：弦网低能谱线性 → 涌现洛伦兹协变 |
| **Spin-2为什么出现** | 坐标重参数化不变性 → 对称张量场 → d=4下TT规范剩2个偏振 |
| **Einstein方程为什么出现** | 弦网自由能的二阶展开 + 长波极限 + 微分同胚不变性 → 唯一形式 |

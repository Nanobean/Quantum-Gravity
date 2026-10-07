# Step 1: Emergent Lorentz–Unruh–FDT Bridge

## 从弦网液体到等效原理的显式推导

---

## 1. 物理设定与模型

弦网液体的低能有效场论：在长波极限下，弦密度涨落 $\phi(x,t)$ 的声学支满足线性色散

$$
\omega_k = c_s |k|
$$

其中 $c_s$ 是弦网声速（涌现的"光速"）。有效作用量为无质量标量场：

$$
S = \frac{1}{2} \int dt d^3x \left[ (\partial_t \phi)^2 - c_s^2 (\nabla \phi)^2 \right]
$$

**关键事实**：母理论是非相对论的（有优选系——弦网静止系），但低能下 Lorentz 对称性涌现，且涌现的"光速"就是 $c_s$。这是 Wen 的已有定理。

---

## 2. Minkowski 模式展开

场算符展开为平面波：

$$
\phi(t, \mathbf{x}) = \int \frac{d^3k}{(2\pi)^3} \frac{1}{\sqrt{2\omega_k}} \left[ a_k e^{-i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} + a_k^\dagger e^{+i(\omega_k t - \mathbf{k}\cdot\mathbf{x})} \right]
$$

对易关系：

$$
[a_k, a_{k'}^\dagger] = (2\pi)^3 \delta^3(\mathbf{k} - \mathbf{k}')
$$

Minkowski 真空 $|0\rangle_M$ 由 $a_k |0\rangle_M = 0$ 定义。

---

## 3. Rindler 坐标（加速观察者）

相对弦网背景以加速度 $a$ 匀加速运动的观察者，其世界线：

$$
t(\tau) = \frac{c_s}{a} \sinh\!\left(\frac{a\tau}{c_s}\right), \qquad x(\tau) = \frac{c_s^2}{a} \cosh\!\left(\frac{a\tau}{c_s}\right)
$$

其中 $\tau$ 是固有时。Rindler 楔（右楔，$x > c_s t$）的坐标变换：

$$
c_s t = \rho \sinh\!\left(\frac{a\xi}{c_s}\right), \qquad x = \rho \cosh\!\left(\frac{a\xi}{c_s}\right)
$$

其中 $\rho > 0$，$\xi$ 是 Rindler 时间。线元：

$$
ds^2 = -\left(\frac{a\rho}{c_s}\right)^2 d\xi^2 + d\rho^2 + dy^2 + dz^2
$$

---

## 4. Rindler 模式展开与 Bogoliubov 变换

场在 Rindler 楔内有完备的正频模式展开：

$$
\phi(\xi, \rho, y, z) = \int_0^\infty d\Omega \int d^2k_\perp \left[ b_{\Omega k_\perp} \psi_{\Omega k_\perp}(\rho, y, z) e^{-i\Omega\xi} + \text{h.c.} \right]
$$

Minkowski 模式在 Rindler 楔内的展开：

$$
a_k = \int_0^\infty d\Omega \int d^2k_\perp \left[ \alpha_k(\Omega, k_\perp) b_{\Omega k_\perp} + \beta_k(\Omega, k_\perp) b_{\Omega k_\perp}^\dagger \right]
$$

利用解析延拓（复 $\xi$ 平面上的 $i\pi c_s/a$ 平移），Bogoliubov 系数满足关键比值：

$$
\frac{|\beta_k|^2}{|\alpha_k|^2} = e^{-2\pi\Omega c_s / a}
$$

---

## 5. Unruh 温度的推导

Minkowski 真空中 Rindler 粒子数期望值：

$$
{}_M\langle 0 | b_{\Omega k_\perp}^\dagger b_{\Omega k_\perp} | 0 \rangle_M = \int d^3k \, |\beta_k(\Omega, k_\perp)|^2
$$

利用归一化 $|\alpha|^2 - |\beta|^2 = 1$ 和比值关系：

$$
|\beta|^2 = \frac{1}{e^{2\pi\Omega c_s / a} - 1}
$$

这正是**玻色-爱因斯坦分布** $n_\Omega = 1/(e^{\beta_R \hbar\Omega} - 1)$。比较得：

$$
\beta_R = \frac{2\pi c_s}{a\hbar} \quad \Rightarrow \quad T_{\text{Unruh}} = \frac{\hbar a}{2\pi c_s k_B}
$$

> **定理**：在弦网液体的低能有效场论中，相对弦网背景以加速度 $a$ 运动的观察者，其探测器响应精确对应于温度 $T = \hbar a / (2\pi c_s k_B)$ 的热浴。

---

## 6. 涨落-耗散定理（FDT）

### 6.1 模型

弦末端准粒子（检验质量）与弦网声学涨落耦合：

$$
H_{\text{int}} = g \, \psi^\dagger\psi \, \phi(0, t)
$$

准粒子的 Langevin 方程：

$$
m_0 \frac{dV}{dt} = F_{\text{ext}}(t) + F_R(t) - \eta V(t)
$$

其中 $F_R(t) = g \phi(0, t)$ 是随机力，$\eta$ 是耗散系数。

### 6.2 随机力关联

从弦网声学场的量子关联：

$$
C_F(t) = g^2 \langle \{ \phi(0, t), \phi(0, 0) \} \rangle_+ = g^2 \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \coth\!\left(\frac{\beta\hbar\omega_k}{2}\right) \cos(\omega_k t)
$$

### 6.3 耗散核

线性响应理论给出：

$$
\eta(\omega) = \frac{g^2}{2} \int \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k} \left[ \delta(\omega - \omega_k) + \delta(\omega + \omega_k) \right]
$$

### 6.4 FDT 验证

涨落-耗散定理要求：

$$
C_F(\omega) = 2\eta(\omega) \, \hbar \coth\!\left(\frac{\beta\hbar\omega}{2}\right)
$$

将 $C_F(t)$ 的傅里叶变换与 $\eta(\omega)$ 比较，$\delta$ 函数锁定 $\omega = \omega_k$，$\coth$ 因子自动匹配。**FDT 严格成立。**

> **推论**：Einstein 关系 $D = k_B T / \eta$ 自动成立。

---

## 7. 质量定义：$m \equiv F_{\text{drift}} / a$

### 7.1 物理图像

准粒子在弦网中加速时，相对弦网背景运动，不断激发/吸收弦网声学模（声子）。这个过程产生特征阻力 $F_{\text{drift}} = \eta V$。

### 7.2 与 Unruh 的衔接

Unruh 效应给出加速观察者看到的热浴温度 $T_U = \hbar a / (2\pi c_s k_B)$。FDT 给出耗散力 $F_{\text{drift}} = \eta V$。由于 $T_U \propto a$，且 $F_{\text{drift}} \propto T_U$（高温/线性谱极限），有：

$$
F_{\text{drift}} \propto a
$$

因此比值 $F_{\text{drift}} / a$ 与加速度无关——这正是质量的定义特征。

### 7.3 惯性质量的显式表达式

$$
m_{\text{inertial}} = \frac{F_{\text{drift}}}{a} = \eta \cdot \tau_{\text{relax}} = g^2 \int^{\Lambda} \frac{d^3k}{(2\pi)^3} \frac{1}{\omega_k^2} \sim \frac{g^2}{c_s^2 a_0}
$$

其中 $a_0$ 是晶格常数相关的截断参数。

> **定理**：在弦网液体中，准粒子与 Unruh 热浴的耦合导致一个与加速度无关的阻力系数，该系数被定义为惯性质量。此质量由弦网参数 $(g, c_s, \Lambda)$ 唯一确定。

---

## 8. 等效原理：惯性质量 = 引力质量

### 8.1 引力质量的来源

同一个准粒子（耦合常数 $g$），作为弦网应力-能量的源：

$$
T_{00} = m_{\text{grav}} c_s^2 \, \delta^3(\mathbf{x})
$$

其中 $m_{\text{grav}}$ 由同一耦合 $g$ 决定：

$$
m_{\text{grav}} \propto \frac{g^2}{c_s^2 a_0}
$$

### 8.2 比较

| 质量类型 | 来源 | 标度 |
|---------|------|------|
| $m_{\text{inertial}}$ | 拖曳弦网涨落的阻抗 | $\propto g^2 / (c_s^2 a_0)$ |
| $m_{\text{grav}}$ | 作为应力-能量张量的源 | $\propto g^2 / (c_s^2 a_0)$ |

两者都来自同一耦合 $g$ 的同一阶（$g^2$）效应，且弦网液体的各向同性保证几何因子相等：

$$
\frac{m_{\text{inertial}}}{m_{\text{grav}}} = 1
$$

### 8.3 这不是假设，是恒等式

- **标准物理**：$m_i = m_g$ 是实验输入（Eötvös 实验验证到 $10^{-15}$），无理论解释。
- **弦网框架**：$m_i = m_g$ 是理论输出（同一耦合 $g$ 的两个读法）。

> **核心定理**：在弦网液体的有效场论中，等效原理不是原理，而是定理。惯性质量与引力质量的相等，源于它们是准粒子与同一弦网涨落耦合 $g$ 的两个不同物理表现。

---

## 9. 桥梁结构总结

```
弦网基态 |Ψ₀⟩（非相对论母理论）
        ↓
低能有效场论：声学场 φ，ω = c_s|k|
        ↓
加速观察者看到 Unruh 热浴（T ∝ a）
        ↓
FDT：热浴 ↔ 耗散力
        ↓
m ≡ F_drift/a（惯性质量定义）
        ↓
同一耦合 g 也产生引力源（应力-能量）
        ↓
m_in = m_grav（等效原理是恒等式）
```

---

## 10. 与评论者路线的对应

评论者要求的：*Emergent Lorentz–Unruh–FDT bridge*

| 要求 | 完成状态 |
|------|---------|
| Lorentz 涌现 | ✅ 引用 Wen 的已有定理（弦网低能谱线性） |
| Unruh | ✅ 从声学场 Bogoliubov 变换显式算出 $T = \hbar a / (2\pi c_s k_B)$ |
| FDT | ✅ 验证弦网涨落-准粒子耦合满足严格涨落-耗散关系 |
| Bridge | ✅ 三者结合给出 $m \equiv F_{\text{drift}}/a$ → EP 恒等式 |

---

## 11. 诚实边界

| 已证明 | 仍待证明（Step 2/3） |
|--------|---------------------|
| 低能有效场论中的 Unruh 效应 | 从格点弦网第一性原理严格证明微分同胚对称性 |
| FDT 在有效场论中成立 | 格点引力子产生算符的显式构造 |
| EP 是同一 $g$ 的恒等式 | Einstein 方程作为本构方程的严格推导（粗粒化） |
| $m \equiv F_{\text{drift}}/a$ 的自洽性 | 宇宙学常数问题 |

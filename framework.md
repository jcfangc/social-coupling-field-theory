# 社会三场论：精炼版理论与定义（含能量—信息桥接）

## 0) 目标与视角

* 用**物质 ρₘ**、**能量 ρₑ**、**信息 ρᵢ**三场，在一维环形空间 $S^1$ 上刻画社会动力学。
* **守恒不作硬约束**；以**对称性**（时间/空间平移不变、相互作用形式不变）为基本原则。
* 个体/组织 = 三场的**局部激发态**（涌现的稳定峰/结构）。

---

## 1) 基本空间与变量

* 空间：环 $x\in[0,L)$，周期边界。时间 $t\ge 0$。
* 场：$\rho_k(x,t)$, $k\in\{m,e,i\}$。
* 可观测量：$\langle \rho_k\rangle(t)=\frac1L\int_0^L\rho_k\,dx$；综合景观函数

  $$
  F(t)=\int_0^L\big(w_m\rho_m+w_e\rho_e+w_i\rho_i\big)\,dx
  $$

  （权重 $w_\*$ 可随时代校准）。

---

## 2) 公理（Axioms）

**A1** 三场是社会的基本表述；个体为场激发态而非外加粒子。
**A2** 动力学由**对称性不变**的统一函数（拉格朗日/势泛函）生成。
**A3** 信息的**有效增长**（不确定性下降/相对熵下降）需要能量代价（Landauer 下限）。
**A4** 信息存在依赖物质载体（结构/存储介质）。
**A5** 能量与物质可相互转化（宏观上通过供能与资源开采/消耗反映，微观等价由 $E=mc^2$ 奠基）。
**A6** 社会处于**带噪声的最优化**过程：在约束下使 $F(t)$ 长期上升（随机梯度式攀升）。

---

## 3) 作用量与“生成器”

现实社会具有耗散与噪声，更合适采用\*\*“拉格朗日 + 耗散”\*\*框架（Onsager–Machlup/广义最小作用）：

$$
S=\int_0^T\!\!\int_0^L\Big(\underbrace{\mathcal L(\rho,\partial_t\rho,\nabla\rho)}_{\text{生成结构}}\;-\;\underbrace{\mathcal R(\partial_t\rho)}_{\text{耗散代价}}\Big)\,dx\,dt
$$

* 变分给出**耗散版欧拉–拉格朗日**：

$$
\frac{d}{dt}\frac{\partial\mathcal L}{\partial(\partial_t\rho_k)}-\frac{\partial\mathcal L}{\partial\rho_k}
+\frac{\partial\mathcal R}{\partial(\partial_t\rho_k)}=0,\quad k\in\{m,e,i\}.
$$

* 直觉：$\mathcal L$ 编码“能动性−约束”的结构规律；$\mathcal R$ 编码现实代价（能量/摩擦/组织成本）。

---

## 4) 最小工作式：反应–扩散 + Landauer 耦合

在环上给出可模拟的最小方程组（满足空间/时间平移对称）：

$$
\begin{aligned}
\partial_t\rho_m &= D_m\nabla^2\rho_m \;+\; \alpha\,\rho_e\,\rho_i\;-\;\delta_m\rho_m \\
\partial_t\rho_e &= D_e\nabla^2\rho_e \;+\; P_{\text{ext}} \;-\; \underbrace{\frac{k_BT\ln2}{\eta}\,\partial_t I_{\text{eff}}}_{\text{信息增益的能量代价}}\;-\;\delta_e\rho_e \\
\partial_t\rho_i &= D_i\nabla^2\rho_i \;+\; \underbrace{\eta\,\frac{P_{\text{info}}}{k_BT\ln2}}_{\text{Landauer 受限的信息生成}}\;-\;\delta_i\rho_i \;+\;\sigma\,\xi(x,t)
\end{aligned}
$$

* $D_\*$：扩散系数；$\alpha$：信息×能量对物质生产的协同；$\delta_\*$：耗散/折旧。
* $P_{\text{ext}}$：外部供能；$P_{\text{info}}\le \chi\,\rho_e$：分配给信息处理的功率（$\chi$ 为分配因子）。
* $\eta\in(0,1]$：信息生成效率；$\xi$ 为零均值噪声。
* **关键信息量定义**（与“有效不确定性”挂钩）：

  $$
  I_{\text{eff}}(t)=\int_0^L \underbrace{D_{\mathrm{KL}}\!\big(p(x,t)\,\|\,p_{\text{ref}}(x)\big)}_{\text{相对熵/互信息代理}}\,dx
  $$

  ——用于把“**可用/结构化信息**的净增加”与能量代价捆绑（Landauer 下限）。

> 注：白噪声导致的“熵增”不计入 $I_{\text{eff}}$（它不降低不确定性），符合你“信息量=不确定性被消除”的语义。

---

## 5) 势泛函/优化视角（等价表述）

也可引入**社会势泛函**（凸优化直觉）：

$$
\Phi[\rho]=\int_0^L\!\Big(\tfrac{a_m}{2}(\nabla\rho_m)^2+\tfrac{a_e}{2}(\nabla\rho_e)^2+\tfrac{a_i}{2}(\nabla\rho_i)^2+V(\rho_m,\rho_e,\rho_i)\Big)\,dx,
$$

令动力学为**带噪声的梯度流**：

$$
\partial_t\rho_k=-M_k\,\frac{\delta\Phi}{\delta\rho_k}+\text{noise}+\text{源/耗散},
$$

与上面的反应–扩散在合适选取 $V$ 时等价；体现你提出的“**随机游走的凸优化**”。

---

## 6) 三者耦合的物理合法性（桥接条款）

* **能量↔物质**：宏观供能/资源转化（微观由 $E=mc^2$ 奠基）。
* **能量↔信息**：**Landauer 原理**（每减少 1 bit 不确定性，最低代价 $k_BT\ln2$）。
* **信息↔物质**：信息依赖物质载体与结构（DNA/存储器/制度文本等）。
  → 三者形成闭环耦合，且在方程中以**显式项**出现（见 §4）。

---

## 7) 校准与验证（如何“落地成学科”）

* **待校准参数**：$\alpha,\eta,\chi,\delta_\*,D_\*,M_k,a_k$ 与势函数 $V$ 的系数。
* **数据锚点**：工业革命（高 $\alpha$、高 $P_{\text{ext}}$）、信息化时代（高 $\eta,\chi$）、能源危机（高 $\delta_e$）、战时动员（$P_{\text{ext}}$ 脉冲）。
* **验证**：回放历史时间窗，看 $F(t)$、$\langle\rho_k\rangle$、$I_{\text{eff}}$ 是否复现拐点与尺度关系。

---

## 8) 你要记住的“最小语义”

* **拉格朗日量**：单位时空上的“能动性−约束”的结构表达（生成律）。
* **欧拉–拉格朗日**：把生成律变成**演化方程**；加耗散即为现实社会版。
* **Landauer**：把“**有效信息增益**”的速率与**能量功率**以下界方式严密绑定。
* **整体对称性**而非逐点守恒，是我们的一等公民。

---

如果你想把它立刻跑起来，我可以给你一个**最小可运行的 Python 原型**：一维环上的三场反应–扩散（含 Landauer 约束），可视化 $\rho_m,\rho_e,\rho_i$ 与 $I_{\text{eff}}$ 的时间–空间纹理图；并留好接口用于历史数据的参数拟合。

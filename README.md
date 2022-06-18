# An-Intro-to-Applied-and-Environmental-Geophysics
Note
## 7.1 Intro

有各種不同的方法可以測定電阻率

相互連貫但各自獨立的解釋，代表所得到的模型是很棒的

如果解釋相互衝突，就要回去檢查每個階段的資料取得、處理和解釋

## 7.2 Basic principles

### 7.2.1 電阻率

材料阻止電流通過，導致電壓下降，就是電阻

> 電阻(R) : R = V/I = ρL/A
> 
> 電阻率(ρ) : ρ(Ωm) = E(V/m)/J(A/m^2) = VA/IL 只和材料、溫度有關，和長度、面積無關
> 
> 導電率(σ) : σ(S/m) = 1/ρ

當電流密度(J)太高，會破壞線性關係

Two media in one cube, then the cube is anisotropy

這個方塊的導電性會受到兩介質的比例和指向的影響

非均質常數 = ρmax/ρmin (lied between 1-2)

岩石中有三種方法可以導電
1. 電解傳導
2. 電子傳導
3. 介電質傳導 : 作為絕緣體、電容。藉由原子中的電子的稍稍移動來導電。在光譜誘發極化SIP、CR、CC中很重要。

在岩石中，pore fluids 作為電解質，礦物本身不太導電(可以忽略)

火成岩的電阻率最高；變質岩居中；沉積岩最低

岩石越老電阻率越高，因為經過再結晶和壓密作用

>Archie’s law relates the effective conductivity to the fluid conductivity σL, fluid saturation sL, and porosity εp:
>
>![image](https://user-images.githubusercontent.com/105845318/170693293-36121064-5c52-45f5-a6ea-846d5e620a54.png)
>
>here, m is the cementation exponent, it describes the connectivity of the pores. m normally between 1.3 and 2.5 for most sedimentary rocks and is close to 2 for sandstones. The lower limit m = 1 represents a volume average of the conductivities of a fully saturated, insulating (zero conductivity) porous matrix, and a conducting fluid. The saturation coefficient n is normally close to 2. The ratio F = σL/σ is called the formation factor.
Archie’s law does not take care of the relative permittivity of either fluids or solids, so the effective relative permittivity of the porous medium is normally consider as εr = 1.

>For rocks composed of non-conducting matrix minerals and saturated with water
>
>![image](https://user-images.githubusercontent.com/105845318/170694793-b2e9adc8-0507-4283-9f54-e521a6a2f9be.png)
>
>where φ is the porosity (ratio of void volume/total volume), and A and m are constants that depend on the geometry of the pores. For many rocks, A = about 1 and m = about 2. See Keller, G.V. (1982) for a broader discussion. Papers discussing various A and m values for specific rocks (shaly sands, clean sandstones, etc.)
>
>Archie's Law is not valid for rocks containing a significant percentage of clay.  Clay provides for conductive matrix, rendering a fundamental assumption invalid.  Graphite, native metals, and minerals with metallic lusters are also electrical conductors, but these are far scarcer than clays.



> Massive form(high ρ) >> Individual crystals(low ρ) 
> 
> eg. pyrite, galena, magnetite
> 
> Pure(high ρ) >> Combined with impuritie(low ρ)
> 
> eg. hematite, sphalerite
> 
> Graphite may reduce ρ
> 
> Rocks have variable composition eg. sedimentary rocks with gradational facies >> ρ change as % change

地電阻法探測的目的，就是要找到電阻率模型

視電阻率(ρa) : 是現場測得的電阻率。受電阻(R)、電極陣列所造成的幾何因子(K)影響。

### 7.2.2 地球中的電流

單一電極導入一電流，求電位 V(r) = Iρ/2πr = I/2πσr

![image](https://user-images.githubusercontent.com/105845318/170485501-88852ec1-a47e-4bd1-ab36-0c5ce7734bd7.png)

導入電流處(r=0)的電位為無限大，隨著r的增加電位會減少

![image](https://user-images.githubusercontent.com/105845318/170485734-3c6b5ea5-6f33-44c2-995a-f7c9e4dabb8c.png)

<https://gpg.geosci.xyz/content/DC_resistivity/DC_basic_principles_current_voltage_halfspace.html>

## 7.3 電極配置與幾何因素

### 7.3.1 General case

>Geometric factor (K) : ρa = Kg*R where R = δV/I
>
>K = 2π [ 1/AM - 1/MB - 1/AN + 1/NB ] (代表電極的幾何排列)
>
>The generalized formula for calculating Kg for a four-electrode configuration is: Kg = 2π(1/C1P1 – 1/C1P2 – 1/C2P1 + 1/C2P2)1 where C1 and C2, and P1 and P2 are the current and potential electrode positions respectively.

![image](https://user-images.githubusercontent.com/105845318/170714862-4b6e64de-f22e-46d7-be54-d18a4cba6366.png)
 
When AB/z = 2, there will be 50% current flow through the depth z

So very deep = telemetering

利用 Vp = Va + Vb 的性質，可以推導出電阻率的公式 

### 7.3.2 電極配置

> Most commonly used electrode configurations
>  1. Wenner arrays : main response is largely flat/ has a high vertical resolution
>     1. Standard Wenner
>     2. Offset Wenner : easy to use/ (+ areas)+(- areas)/2 can reducng the error due to a lateral inhomogenies.
>     3. Lee partitioning array (Not an common one) : to reduce near-surface lateral inhomogeneities 
>  2. Schlumberger arrays : main response is largely flat, but 上凹/ has a high vertical resolution
>     1. Standard Schlumberger
>  3. Dipoledipole arrays : has a poor vertical resolution(lobate)/ particularly sensitive to deep area/ unsuitable for depth sounding(電極間距interelectrode和測線長度有很大的關係)
>     1. Normal(axial or polar)
>     2. Equatorial
>     3. Square(special form of equatorial) : particularly 

關於電極配置的選擇，除了空間、勞力因素之外。對於測向不均勻的敏感度、傾角介面也是非常重要的因素。

Signal contribution sections : 顯示地底下的電位等值線(Contour line)

我們將電極配置中的距離參數(a)，帶入K公式以後，就可以得到，不同電極配置，所對應的視電阻率公式。

先跳到 7.5
麒書要教我資料處理了

## 7.5 解釋方法

Vertical sounding field curves 可以用圖形、半數值半圖形、電腦模型(數值)來解釋

電腦模型最為嚴謹，但可能會過度解釋

Field curve 會有不明顯的反曲點或頂點，解釋者需要判斷他有多重要

一個雜訊多的 field curve 要先得到一個平滑的圖形，在用數值方法來解釋

### 7.5.1 定性研究

First to identify the curve shapes
 1. 有六種大致的模型
 2. X軸可以分為三-四個"層"來看
 3. log-log 曲線的傾斜若超過45° = error in data
 4. ρ1ρ2ρ3的相對大小是解釋的起頭
 5. 如果其中一層非常薄，那這層可能不存在
 6. 轉折點不代表最大最小值

### 7.5.2 Master Curve

前提假設 : 地表水平延伸、越深越厚
條件限制 : Master curve 最多只能用到四層
作圖過程 : 有點複雜，自己看課本

### 7.5.3 Curve matching by computer

The method called 'liner digital filter'


---
theme: ./
layout: cover
class: text-left
transition: slide-left
mdc: true
authors:  # First author should be the presenter
  - Xuliang Zhu: ["TDLI"]
  - Yifan Zhu: ["INPAC"] 

meeting: "Dark SHINE Calorimeter R&D Weekly Meeting"
preTitle: "DAna ActsSequencer v0.3"
---

<br>

<img id="ATLAS" src="/DarkSHINE/DarkSHINE-Logo.png"> </img>

<style scoped>
#ATLAS {
  width: 160px;
  position: absolute;
  right: 3%;
  bottom: 4%;
  /* background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 15%, #146b8c 50%); */
}
</style>

---
layout: pageBar
hideInToc: true
---

# Outline

<br>

<div class="flex justify-center items-center" style="height: 50vh;">

### <Toc />
</div>

---
layout: pageBar
---

# Track Efficency

## Tagging Track Number

| Eff | Inclusive | Signal 5 MeV |
| ---      | ---   | --- |
| Acts Tagging | **99.94%** | **99.94%** |
| DarkSHINE Tagging | 99.69%| 99.78% |
| Acts Recoil  | **99.76%** | 80.49 %|
| DarkSHINE Recoil | 99.27% | **87.55%** |

<div grid="~ cols-2 gap-2">
<Transform :scale="0.5">
<PlotlyGraph filePath="plots/json/Acts_TagTrk_No_cut1.json"/>
</Transform>
<Transform :scale="0.5">
<PlotlyGraph filePath="plots/json/Acts_RecTrk_No_cut2.json"/>
</Transform>
</div>


---
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Tagging Tracker at Truth P = 8±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dTagTrk2_pp_8_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_TagTrk_P_8_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 1±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_1_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_1_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 2±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_2_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_2_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 3±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_3_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_3_cut2.json"/>
</Transform>

</div>


---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 4±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_4_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_4_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 5±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_5_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_5_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 6±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_6_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_6_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 7±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_7_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_7_cut2.json"/>
</Transform>

</div>

---
hideInToc: true
layout: pageBar
---

# P<sub>Track</sub> Reconstruction Performance

## Recoil Tracker at Truth P = 8±0.5 GeV

<div grid="~ cols-2 gap-2">

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dRecTrk2_pp_8_cut2.json"/>
</Transform>

<Transform :scale="0.7">
<PlotlyGraph filePath="plots/json/dActs_RecTrk_P_8_cut2.json"/>
</Transform>

</div>


---
layout: pageBar
---

# ActsSequencer Development Plan

<br>

```mermaid
%%{init: { 'theme': 'dark' } }%%
timeline
    section Apr. 1 - Apr. 7
        v0.1 ✅ : Baseline track reconstruction
        v0.2 ✅ : Fix hard-coded parts
    section Apr. 8 - Apr. 14
        v0.3 ✅ : Add non-constant magnetic field
        v0.4 ✅ : Add vertexing
    section Apr. 15 - Apr. 21
        v0.4 [WIP] : Replace the ECAL seed by the Acts track
        v1.0 : Add default seeding algorithm
```

---
hideInToc: true
layout: center
class: "text-center"
---

# Thanks

[Git Repo](https://code.ihep.ac.cn/darkshine/darkshine-simulation/-/tree/acts-xuliang)


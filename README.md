# DeepBench: Domain-Specific Robustness Evaluation Framework for Vision and Vision-Language Models 

![DeepBench Flowchart](resources/graphical_abstract.svg)  


## Table of Contents
1. [Project Overview](#project-overview)  
2. [Components](#components)  
5. [Usage](#usage)  
6. [Project TAHAI](#project-tahai)  
7. [License](#license)  
8. [Authors & Acknowledgments](#authors--acknowledgments)  

---

## Project Overview  
DeepBench is a benchmarking framework developed under the TAHAI (TrustAdHocAI) project.
It provides:  

- **Systematic evaluation** of image classification models  
- **Quantitative analysis** of model robustness against image perturbations  
- **Visual insights** into performance degradation  

The system consists of two integrated components:  
1. **Benchmark Framework** (Backend): Benchmark models with controlled perturbations  
2. **Analysis Dashboard** (Frontend): Visualizes results and model comparison metrics  

Designed for GPU-accelerated environments, DeepBench supports modern vision-language models including from Hugging Face and Ollama APIs.

---

## Components  

### 🚀 DeepBench Backend  
*Command-line tool for configuration of experiments and running the benchmarks*  

**Core Functionality**:  
- Applies ~17 image transformations across multiple adjustable use-cases  
- Tests models with individual or ramped corruptions
- Stores results in MongoDB (remote) or TinyDB (local)
- TOML-configurable experiments  


### 📊 DeepBench Analysis Frontend  
*Interactive visualization dashboard*  

**Core Functionality**:  
- Model performance comparison across perturbation types and different metrics 
- Use-case specific analysis (Medical, Autonomous Driving, etc.)  

---

## Usage   
- The usage of each submodule is described in more detail in their own README files  

---

## Project TAHAI  
Developed under the TAHAI (TrustAdHocAI) project:  
- Quantifying model robustness boundaries  
- Establishing trust metrics for vision systems  
- Human-AI collaboration frameworks  

**Project Links**:  
- [Paper Submission](https://ki2025.gi.de/calls/call-for-papers) Status: submitted
- [IFAF Project Page](https://www.ifaf-berlin.de/projekte/tahai/)  
- [HTW Research Profile](https://www.htw-berlin.de/forschung/online-forschungskatalog/projekte/projekt/?eid=3418)  
- [KI-Werkstatt Implementation](https://kiwerkstatt.f2.htw-berlin.de/projekte/tahai)  

---

## License  
**MIT License** - See [LICENSE](LICENSE) for details.

---

## Authors & Acknowledgments  
**Team**:  
- Mario Koddenbrock (`Mario.Koddenbrock@HTW-Berlin.de`)  
- Erik Rodner (`Erik.Rodner@HTW-Berlin.de`)  
- David Brodmann (`David.Brodmann@htw-berlin.de`)  
- Rudolf Hoffmann (`Rudolf.Hoffmann@student.htw-berlin.de`)  

**Funding**:  
This research was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) via the Project ApplFM (528483508) and
the Institut für angewandte Forschung Berlin (IFAF, Berlin Institute for Applied Research) via Project TrustAdHocAI (TAHAI).

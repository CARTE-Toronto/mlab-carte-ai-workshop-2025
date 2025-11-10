---
layout: default
---

<style>
/* simple left nav for in-page anchors */
.page-wrap { display: flex; gap: 24px; }
.page-toc { min-width: 220px; border-right: 1px solid #e5e5e5; padding-right: 16px; }
.page-toc h3 { margin-top: 0; font-size: 1rem; }
.page-toc ul { list-style: none; padding-left: 0; margin: 8px 0; }
.page-toc li { margin: 6px 0; }
.page-content-body { flex: 1; }
@media (max-width: 900px) {
  .page-wrap { flex-direction: column; }
  .page-toc { border-right: none; border-bottom: 1px solid #e5e5e5; padding-bottom: 12px; }
}
</style>

<script>
function copyLabCPrompt(btn) {
  const text = document.getElementById('lab-c-prompt').textContent;
  navigator.clipboard.writeText(text).then(function() {
    const originalText = btn.textContent;
    btn.textContent = '✓ Copied!';
    btn.style.background = '#28a745';
    setTimeout(function() {
      btn.textContent = originalText;
      btn.style.background = '#0066cc';
    }, 2000);
  }).catch(function(err) {
    alert('Failed to copy text: ' + err);
  });
}
</script>

<div class="page-wrap">
  <nav class="page-toc" aria-label="Page navigation">
    <h3>Jump to</h3>
    <ul>
      <li><a href="#day-1">Day 1 — Tuesday, Oct 14</a></li>
      <li><a href="#day-2">Day 2 — Wednesday, Oct 15</a></li>
      <li><a href="#day-3">Day 3 — Thursday, Oct 16</a></li>
      <li><a href="#day-4">Day 4 — Friday, Oct 17</a></li>
    </ul>
  </nav>

  <div class="page-content-body" markdown="1">

Thank you for joining the **M-Lab CARTE AI Workshop 2025**. This site now serves as the post-workshop archive so you can revisit lectures, labs, and reference materials at your own pace.

**Workshop Dates:** Tuesday, October 14 to Friday, October 17 2025  
**Hosted by:** [Centre for Analytics and AI Engineering (CARTE)](https://carte.utoronto.ca), University of Toronto  

Use the schedule below to jump directly to recordings, slides, and lab notebooks. For local setup tips and downloading materials in bulk, see the repository `README.md`.

## Workshop Overview

This program covers AI fundamentals through advanced agentic AI systems, with practical applications for business implementation. The recordings, labs, and worksheets remain available for self-guided refreshers and team knowledge transfer.

### Post-Workshop Tips

- Start with the recorded lectures to recap core ideas, then work through the matching labs.
- Each lab notebook includes practice prompts (kept as TODOs) plus solution callouts where available.
- Need a quick refresher? Download the PDF versions in `labs/` for offline reference.
- Share questions or success stories with the CARTE team—contact details are at the bottom of this page.

## Workshop Schedule

### **Day 1: AI Foundation & Data Mastery** — Tuesday, October 14, 2025 {#day-1}

| **Time** | **Session** | **Focus Area** | **Materials** | **Recording** |
|----------|-------------|----------------|---------------|---------------|
| **09:00** | **Lecture A:** AI Landscape Overview | ML • Deep Learning • Generative AI • Autonomous Agents | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_a_ai_landscape_overview.pdf) | [Watch](https://youtu.be/LoMWPXntUV4) |
| **10:45** | **Lab A:** Exploratory Data Analysis | Python fundamentals • NumPy arrays • scikit-learn introduction • Visualization | [Open in Colab](https://colab.research.google.com/github/CARTE-Toronto/mlab-carte-ai-workshop-2025/blob/main/labs/lab_a_exploratory_data_analysis.ipynb) | |
| **13:00** | **Lecture B:** Neural Networks & Optimization | Architecture fundamentals • Training strategies • Performance optimization | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_b_neural_networks_and_optimization.pdf) • [Neuron Visualizer](https://carte-toronto.github.io/visualizations/interactive-neuron-visualizer) • [Gradient Descent Visualizer](https://carte-toronto.github.io/visualizations/gradient-descent-visualizer) | [Watch](https://youtu.be/OG-U7psvVoE) |
| **14:45** | **Lab B:** Data Cleaning and Processing | Missing values • Normalization • One-hot encoding • Class imbalance | [Open in Colab](https://colab.research.google.com/github/CARTE-Toronto/mlab-carte-ai-workshop-2025/blob/main/labs/lab_b_data_cleaning_and_processing.ipynb) • [TensorFlow Playground](https://playground.tensorflow.org) • [CNN Explainer](https://poloclub.github.io/cnn-explainer/) | |

### **Day 2: Generative AI** — Wednesday, October 15, 2025 {#day-2}

| **Time** | **Session** | **Focus Area** | **Materials** | **Recording** |
|----------|-------------|----------------|---------------|---------------|
| **09:00** | **Lecture C:** Large Language Models | Transformer architecture • Training methodologies • Enterprise deployment | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_c_large_language_models.pdf) • [Embedding Visualizer](https://carte-toronto.github.io/visualizations/word-embedding-visualizer) • [Transformer Explainer](https://poloclub.github.io/transformer-explainer/) • [TensorFlow Embedding Projector](https://projector.tensorflow.org/) • [Token Prediction Visualizer](https://carte-toronto.github.io/visualizations/gemini-token-predictor) | [Watch](https://youtu.be/BJxgCXwvLVk) |
| **10:45** | **Lab C:** Visual Workflow Building | System prompts • Reasoning models  • Retrieval-augmented generation | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lab_c_visual_workflow_building.pdf) • [Prompt Template](#lab-c-prompt-template) • [[note]](#ref1) | |
| **13:00** | **Lecture D:** Beyond Text — Multimodal AI | Image • Video • Audio generation • Cross-modal applications | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_d_beyond_text_and_multimodal_ai.pdf) • [Video Generation Demo](https://generative-animation-explainer-871047044699.us-west1.run.app) • [Diffusion Explainer](https://carte-toronto.github.io/visualizations/diffusion-model-demonstrator) | [Watch](https://youtu.be/9CjBZ4bHz9A) |
| **14:45** | **Lab D:** Multimodal Content Creation | Creative AI applications • Business use cases • Technical implementation | [Worksheet](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lab_d_multimodal_content_generation.pdf) • [Link to Google AI Studio](https://aistudio.google.com/) • [Link to Video Generation with Google AI studio](https://aistudio.google.com/prompts/new_video) • [NotebookLM AI Generated Video](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/assets/Neural_Text-to-Speech.mp4) | |

<div id="lab-c-prompt-template" style="margin: 16px 0; padding: 12px; background: #f6f8fa; border: 1px solid #d0d7de; border-radius: 6px;">
<details>
<summary style="cursor: pointer; font-weight: bold; margin-bottom: 8px;">Lab C: System Prompt Template (click to expand)</summary>
<pre id="lab-c-prompt" style="background: white; padding: 12px; border-radius: 4px; overflow-x: auto;">Given the user question and history, construct a short string that can be used for searching a document store. Only generate the query, no meta comments, no explanation Example: Question: what are the events happening today? Query: today's event Example: Question: how about the address? Query: business address of the shop Question: {{ question }} Query:</pre>
<button onclick="copyLabCPrompt(this)" style="padding: 8px 16px; cursor: pointer; background: #0066cc; color: white; border: none; border-radius: 4px; font-size: 14px; font-weight: 500; margin-top: 8px;">📋 Copy to Clipboard</button>
</details>
</div>

<div id="lab-d-outputs" style="margin: 16px 0; padding: 12px; background: #f6f8fa; border: 1px solid #d0d7de; border-radius: 6px;">
<details>
<summary style="cursor: pointer; font-weight: bold; margin-bottom: 8px;">Lab D: Team Outputs — Multimodal Content Gallery (click to expand)</summary>
<div style="background: white; padding: 12px; border-radius: 4px;">

<h4 style="margin-top: 0;">Table 1</h4>
<ul>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%201/Generated%20File%20October%2015%2C%202025%20-%203_24PM.mp4" target="_blank">Video 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%201/Generated%20Image%20October%2015%2C%202025%20-%203_00PM.png" target="_blank">Image 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%201/Generated%20Image%20October%2015%2C%202025%20-%203_11PM.png" target="_blank">Image 2</a></li>
</ul>

<h4>Table 2</h4>
<ul>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%202/MovieAd.mp4" target="_blank">Video 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%202/PosterAdpng.png" target="_blank">Image 1</a></li>
</ul>

<h4>Table 3</h4>
<ul>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%203/Generated%20File%20October%2015%2C%202025%20-%2012_13PM%20(1).mp4" target="_blank">Video 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%203/Image.png" target="_blank">Image 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%203/Terran%20Nature%20Lamp.png" target="_blank">Image 2</a></li>
</ul>

<h4>Table 4</h4>
<ul>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%204/20251015_1517_01k7mmjm6nfqs96sf2zcmdqwbs.mp4" target="_blank">Video 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%204/20251015_1527_01k7mnc9p0fb9tpbe8gcxqqpx4.mp4" target="_blank">Video 2</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%204/a_video_based_on_this_info_product.mp4" target="_blank">Video 3</a></li>
</ul>

<h4>Table 5</h4>
<ul>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%205/Video.mp4" target="_blank">Video 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%205/Logo.png" target="_blank">Image 1</a></li>
<li><a href="https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/lab-d-output/Table%205/Poster.png" target="_blank">Image 2</a></li>
</ul>

</div>
</details>
</div>

### **Day 3: Agentic AI & Technology Evaluation** — Thursday, October 16, 2025 {#day-3}

| **Time** | **Session** | **Details** |
|----------|-------------|---------------|
| **09:00** | **Industry Expert Presentation:** AI Technology Evaluation & Investment | **Led by Eva Lau** (Co-Founder & GP, [Two Small Fish Ventures](https://twosmallfish.vc/)) • [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/assessing_startup_opportunities_in_the_ai_era.pdf) |
| **10:45** | **Lab E:** Advanced Agents | Agentic workflows • Tool integration • Autonomous decision-making • [Worksheet](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lab_e_agent_workflow_exercise.pdf) |
| **13:00** | **Specialized Workshop:** Robotics & AI | **Led by Professor Chi-Guhn Lee and his research team** |

### **Day 4: Implementation & Action Planning** — Friday, October 17, 2025 {#day-4}

| **Time** | **Session** | **Focus Area** | **Materials** | **Recording** |
|----------|-------------|----------------|---------------|---------------|
| **09:00** | **Lecture F:** Agentic Systems | Chain-of-Thought • Hallucination • Scalability | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_f_agentic_systems.pdf) | [Watch](https://youtu.be/PsPvpauptGg) |
| **10:45** | **Lab F:** AI Safety & Ethics | Evaluation frameworks • Risk assessment • Quality assurance |[Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lab_f_ai_safety_and_ethics.pdf) • [Worksheet](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lab_f_safety_workshop.pdf) • [Resumés (Zip File)](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/assets/Resumes.zip) | |
| **13:00** | **Lecture G:** Multi-Agent System Orchestration | Routing • Communication protocols • Complex problem solving | [Slides](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/lecture_g_multi_agent_system_orchestration.pdf) • [Multi-Agent AI Systems Demo](https://carte-toronto.github.io/visualizations/multi-agent-ai-systems) | |
| **14:45** | **Action Clinic:** 90-Day Implementation Roadmap | Strategy development • Team feedback • Executive presentation prep | [Canvas](https://github.com/CARTE-Toronto/mlab-carte-ai-workshop-2025/raw/main/slides/action_clinic_canvas.pdf)| |

## Expert Support & Contact

**Alex Olson** — *Workshop Director*  
[alex.olson@utoronto.ca](mailto:alex.olson@utoronto.ca)  
*Leading AI education initiatives and industry partnerships*

**Rahul Patel** — *Lab Instructor & Content Developer*  
[rahulptel.github.io](https://rahulptel.github.io/)  
[rm.patel@mail.utoronto.ca](mailto:rm.patel@mail.utoronto.ca)  
*PhD Candidate, Stochastic & Multi-Objective Optimization, University of Toronto & Vector Institute*

**Nakul Upadhya** — *Lab Instructor & Content Developer*  
[upadhyan.github.io](https://upadhyan.github.io/index.html)  
[nakul.upadhya@mail.utoronto.ca](mailto:nakul.upadhya@mail.utoronto.ca)  
*PhD Candidate, Interpretable Sequence Models, University of Toronto*

## References

<a id="ref1"></a>[1] Lab C slides are partly adapted from [FlowiseAI: Agentic RAG Tutorial](https://docs.flowiseai.com/tutorials/agentic-rag)

  </div>
</div>
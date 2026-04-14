<br>
<br>
<p align="center">
<img src="assets/EXAONE_Symbol+BI_3d.png" width="400">
<br>
<br>
<br>

<div align="center">
  <a href="https://huggingface.co/collections/LGAI-EXAONE/exaone-45" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/🤗-HuggingFace-FC926C?style=for-the-badge" alt="HuggingFace">
  </a>
  <a href="https://www.lgresearch.ai/blog/view?seq=641" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/📝-Blog-E343BD?style=for-the-badge" alt="Blog">
  </a>
  <a href="http://arxiv.org/abs/2604.08644" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/📑-Technical_Report-684CF4?style=for-the-badge" alt="Technical Report">
  </a>
  <a href="https://github.com/LG-AI-EXAONE/EXAONE-4.5" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/🖥️-GitHub-2B3137?style=for-the-badge" alt="GitHub">
  </a>
  <!-- <a href="#" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/✈️_API-Try_on_FriendliAI-2649BC?style=for-the-badge" alt="FriendliAI">
  </a> -->
</div>

<br>

<br>


## EXAONE 4.5

We introduce EXAONE 4.5, the first open-weight vision language model developed by LG AI Research.
Integrating a dedicated visual encoder into the existing EXAONE 4.0 framework, we expand the model's capability toward multimodality.
EXAONE 4.5 features 33 billion parameters in total, including 1.2 billion parameters from the vision encoder. 
EXAONE 4.5 achieves competitive performance in general benchmark while outperforming SOTA models of similar size in document understanding and Korean contextual reasoning, inheriting powerful language capabilities from our previous language models.

For more details, please refer to the [technical report](http://arxiv.org/abs/2604.08644), [blog](https://www.lgresearch.ai/blog/view?seq=641) and [GitHub](https://github.com/LG-AI-EXAONE/EXAONE-4.5).




## News

- 2026.04.09 : 🚩 We release EXAONE 4.5, the first open-weight vision language model with 33B params. Please check out [the model](https://huggingface.co/collections/LGAI-EXAONE/exaone-45)
- 2025.12.31 : We release 🇰🇷 K-EXAONE, a 236B MoE model with 23B active params, efficiently scaling model capacity with significant enhancement. Please check out [the model](https://huggingface.co/collections/LGAI-EXAONE/k-exaone)!
- 2025.07.15 : We released EXAONE 4.0, a hybrid reasoning model with enhanced usability including 32B and 1.2B. Please check out [these models](https://huggingface.co/collections/LGAI-EXAONE/exaone-40)!
- 2025.03.18: We released the EXAONE Deep, reasoning enhanced language models, including 2.4B, 7.8B, and 32B. Check out [these models](https://huggingface.co/collections/LGAI-EXAONE/exaone-deep)!
- 2024.12.09: We released the EXAONE 3.5 language model series including 2.4B, 7.8B, and 32B instruction-tuned models. Check out [these models](https://huggingface.co/collections/LGAI-EXAONE/exaone-35)!
- 2024.08.07: We released the EXAONE 3.0 7.8B instruction-tuned model. Check out the [model](https://huggingface.co/collections/LGAI-EXAONE/exaone-30)!

## Performance



### Vision-Language Tasks

<table>
	<tr>
		<th style="background: rgba(128,128,128,0.1); text-align: center;"> </th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">EXAONE 4.5 33B (Reasoning)</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">GPT-5 mini (Reasoning: high)</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">Qwen3-VL 32B Thinking</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">Qwen3-VL 235B Thinking</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">Qwen3.5 27B (Reasoning)</th>
	</tr>
	<tr>
		<td align="center">Architecture</td>
		<td align="center">Dense</td>
		<td align="center">-</td>
		<td align="center">Dense</td>
		<td align="center">MoE</td>
		<td align="center">Dense</td>
	</tr>
	<tr>
		<td align="center">Total Params</td>
		<td align="center">33B</td>
		<td align="center">-</td>
		<td align="center">33B</td>
		<td align="center">236B</td>
		<td align="center">27B</td>
	</tr>
	<tr>
		<td align="center">Active Params</td>
		<td align="center">33B</td>
		<td align="center">-</td>
		<td align="center">33B</td>
		<td align="center">22B</td>
		<td align="center">27B</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>STEM / Puzzle</i></td>
	</tr>
	<tr>
		<td align="center">MMMU</td>
		<td align="center">78.7</td>
		<td align="center">79.0</td>
		<td align="center">78.1</td>
		<td align="center">80.6</td>
		<td align="center">82.3</td>
	</tr>
	<tr>
		<td align="center">MMMU-Pro</td>
		<td align="center">68.6</td>
		<td align="center">67.3</td>
		<td align="center">68.1</td>
		<td align="center">69.3</td>
		<td align="center">75.0</td>
	</tr>
	<tr>
		<td align="center">MedXpertQA-MM</td>
		<td align="center">42.1</td>
		<td align="center">34.4</td>
		<td align="center">41.6</td>
		<td align="center">47.6</td>
		<td align="center">62.4</td>
	</tr>
	<tr>
		<td align="center">MathVision</td>
		<td align="center">75.2</td>
		<td align="center">71.9</td>
		<td align="center">70.2</td>
		<td align="center">74.6</td>
		<td align="center">86.0</td>
	</tr>
	<tr>
		<td align="center">MathVista (mini)</td>
		<td align="center">85.0</td>
		<td align="center">79.1</td>
		<td align="center">85.9</td>
		<td align="center">85.8</td>
		<td align="center">87.8</td>
	</tr>
	<tr>
		<td align="center">WeMath</td>
		<td align="center">79.1</td>
		<td align="center">70.3</td>
		<td align="center">71.6</td>
		<td align="center">74.8</td>
		<td align="center">84.0</td>
	</tr>
	<tr>
		<td align="center">LogicVista</td>
		<td align="center">73.8</td>
		<td align="center">70.3</td>
		<td align="center">70.9</td>
		<td align="center">72.2</td>
		<td align="center">77.0</td>
	</tr>
	<tr>
		<td align="center">BabyVision</td>
		<td align="center">18.8</td>
		<td align="center">20.9</td>
		<td align="center">17.4</td>
		<td align="center">22.2</td>
		<td align="center">44.6</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Document Understanding</i></td>
	</tr>
	<tr>
		<td align="center">AI2D</td>
		<td align="center">89.0</td>
		<td align="center">88.2</td>
		<td align="center">88.9</td>
		<td align="center">89.2</td>
		<td align="center">92.9</td>
	</tr>
	<tr>
		<td align="center">ChartQAPro</td>
		<td align="center">62.2</td>
		<td align="center">60.9</td>
		<td align="center">61.4</td>
		<td align="center">61.2</td>
		<td align="center">66.8</td>
	</tr>
	<tr>
		<td align="center">CharXiv (RQ)</td>
		<td align="center">71.7</td>
		<td align="center">68.6</td>
		<td align="center">65.2</td>
		<td align="center">66.1</td>
		<td align="center">79.5</td>
	</tr>
	<tr>
		<td align="center">OCRBench v2</td>
		<td align="center">63.2</td>
		<td align="center">55.8</td>
		<td align="center">68.4</td>
		<td align="center">66.8</td>
		<td align="center">67.3</td>
	</tr>
	<tr>
		<td align="center">OmniDocBench v1.5</td>
		<td align="center">81.2</td>
		<td align="center">77.0</td>
		<td align="center">83.1</td>
		<td align="center">84.5</td>
		<td align="center">88.9</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>General</i></td>
	</tr>
	<tr>
		<td align="center">MMStar</td>
		<td align="center">74.9</td>
		<td align="center">74.1</td>
		<td align="center">79.4</td>
		<td align="center">78.7</td>
		<td align="center">81.0</td>
	</tr>
	<tr>
		<td align="center">BLINK</td>
		<td align="center">68.8</td>
		<td align="center">67.7</td>
		<td align="center">68.5</td>
		<td align="center">67.1</td>
		<td align="center">71.6</td>
	</tr>
	<tr>
		<td align="center">HallusionBench</td>
		<td align="center">63.7</td>
		<td align="center">63.2</td>
		<td align="center">67.4</td>
		<td align="center">66.7</td>
		<td align="center">70.0</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Korean</i></td>
	</tr>
	<tr>
		<td align="center">KMMMU</td>
		<td align="center">42.7</td>
		<td align="center">42.6</td>
		<td align="center">37.8</td>
		<td align="center">42.1</td>
		<td align="center">51.7</td>
	</tr>
	<tr>
		<td align="center">K-Viscuit</td>
		<td align="center">80.1</td>
		<td align="center">78.5</td>
		<td align="center">78.5</td>
		<td align="center">83.9</td>
		<td align="center">84.0</td>
	</tr>
	<tr>
		<td align="center">KRETA</td>
		<td align="center">91.9</td>
		<td align="center">94.8</td>
		<td align="center">90.3</td>
		<td align="center">92.8</td>
		<td align="center">96.5</td>
	</tr>
</table>


### Language-only Tasks

<table>
	<tr>
		<th style="background: rgba(128,128,128,0.1); text-align: center;"> </th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">EXAONE 4.5 33B (Reasoning)</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">GPT-5 mini (Reasoning: high)</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">K-EXAONE 236B (Reasoning)</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">Qwen3-VL 235B Thinking</th>
		<th style="background: rgba(128,128,128,0.1); text-align: center;">Qwen3.5 27B (Reasoning)</th>
	</tr>
	<tr>
		<td align="center">Architecture</td>
		<td align="center">Dense</td>
		<td align="center">-</td>
		<td align="center">MoE</td>
		<td align="center">MoE</td>
		<td align="center">Dense</td>
	</tr>
	<tr>
		<td align="center">Total Params</td>
		<td align="center">33B</td>
		<td align="center">-</td>
		<td align="center">236B</td>
		<td align="center">236B</td>
		<td align="center">27B</td>
	</tr>
	<tr>
		<td align="center">Active Params</td>
		<td align="center">33B</td>
		<td align="center">-</td>
		<td align="center">23B</td>
		<td align="center">22B</td>
		<td align="center">27B</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Reasoning</i></td>
	</tr>
	<tr>
		<td align="center">AIME 2025</td>
		<td align="center">92.9</td>
		<td align="center">91.1</td>
		<td align="center">92.8</td>
		<td align="center">89.7</td>
		<td align="center">93.5</td>
	</tr>
	<tr>
		<td align="center">AIME 2026</td>
		<td align="center">92.6</td>
		<td align="center">92.4</td>
		<td align="center">92.2</td>
		<td align="center">89.4</td>
		<td align="center">90.8</td>
	</tr>
	<tr>
		<td align="center">GPQA-Diamond</td>
		<td align="center">80.5</td>
		<td align="center">82.3</td>
		<td align="center">79.1</td>
		<td align="center">77.1</td>
		<td align="center">85.5</td>
	</tr>
	<tr>
		<td align="center">LiveCodeBench v6</td>
		<td align="center">81.4</td>
		<td align="center">78.1</td>
		<td align="center">80.7</td>
		<td align="center">70.1</td>
		<td align="center">80.7</td>
	</tr>
	<tr>
		<td align="center">MMLU-Pro</td>
		<td align="center">83.3</td>
		<td align="center">83.3</td>
		<td align="center">83.8</td>
		<td align="center">83.8</td>
		<td align="center">86.1</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Agentic Tool Use</i></td>
	</tr>
	<tr>
		<td align="center">τ<sup>2</sup>-Bench (Retail)</td>
		<td align="center">77.9</td>
		<td align="center">78.3</td>
		<td align="center">78.6</td>
		<td align="center">67.0</td>
		<td align="center">84.7</td>
	</tr>
	<tr>
		<td align="center">τ<sup>2</sup>-Bench (Airline)</td>
		<td align="center">56.5</td>
		<td align="center">60.0</td>
		<td align="center">60.4</td>
		<td align="center">62.0</td>
		<td align="center">67.5</td>
	</tr>
	<tr>
		<td align="center">τ<sup>2</sup>-Bench (Telecom)</td>
		<td align="center">73.0</td>
		<td align="center">74.1</td>
		<td align="center">73.5</td>
		<td align="center">44.7</td>
		<td align="center">99.3</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Instruction Following</i></td>
	</tr>
	<tr>
		<td align="center">IFBench</td>
		<td align="center">62.6</td>
		<td align="center">74.0</td>
		<td align="center">67.3</td>
		<td align="center">59.2</td>
		<td align="center">76.5</td>
	</tr>
	<tr>
		<td align="center">IFEval</td>
		<td align="center">89.6</td>
		<td align="center">92.8</td>
		<td align="center">89.7</td>
		<td align="center">88.2</td>
		<td align="center">95.0</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Long Context Understanding</i></td>
	</tr>
	<tr>
		<td align="center">AA-LCR</td>
		<td align="center">50.6</td>
		<td align="center">68.0</td>
		<td align="center">53.5</td>
		<td align="center">58.7</td>
		<td align="center">67.3</td>
	</tr>
	<tr>
		<td align="center" colspan='7' style="background: linear-gradient(90deg, rgba(252,146,108,0.3) 0%, rgba(227,67,189,0.3) 50%, rgba(104,76,244,0.3) 100%); font-weight: bold; height:32px; padding-top:2px; padding-bottom:2px;"><i>Korean</i></td>
	</tr>
	<tr>
		<td align="center">KMMLU-Pro</td>
		<td align="center">67.6</td>
		<td align="center">72.5</td>
		<td align="center">67.3</td>
		<td align="center">71.1</td>
		<td align="center">73.0</td>
	</tr>
	<tr>
		<td align="center">KoBALT</td>
		<td align="center">52.1</td>
		<td align="center">63.6</td>
		<td align="center">61.8</td>
		<td align="center">51.1</td>
		<td align="center">54.9</td>
	</tr>
</table>




## Quickstart


### Serving EXAONE 4.5

For better inference speed and memory usage, it is preferred to serve the model using optimized inference engines. The EXAONE 4.5 model is supported by various frameworks, including TensorRT-LLM, vLLM, SGLang, and llama.cpp. Support will be expanded in the future.

Practically, you can serve the EXAONE 4.5 model with 256K context length on **single H200 GPU**, or **4x A100-40GB GPUs** by using a tensor-parallelism.


### TensorRT-LLM

TensorRT-LLM provides zero day support for EXAONE 4.5. Transformers library of our fork is required to utilize EXAONE 4.5 model.
You can install Transformers by running the following commands:

```bash
pip install git+https://github.com/nuxlear/transformers.git@add-exaone4_5
```

Please refer to the official [installation guide](https://github.com/NVIDIA/TensorRT-LLM?tab=readme-ov-file#getting-started), and [EXAONE documentations](https://github.com/NVIDIA/TensorRT-LLM/tree/main/examples/models/core/exaone), and [EXAONE 4.5 PR](https://github.com/NVIDIA/TensorRT-LLM/pull/12873) for the detail.

After you install the TensorRT-LLM, you can launch the server with the following code snippet. You can remove unnecessary arguments from the snippet.

```bash
trtllm-serve LGAI-EXAONE/EXAONE-4.5-33B \
    —tp_size 2 \
    —port 8000 \
    —reasoning_parser qwen3

```

An OpenAI-compatible API server will be available at http://localhost:8000/v1.


### vLLM

Both Transformers and vLLM of our forks are required to utilize EXAONE 4.5 model.
You can install the requirements by running the following commands:

```bash
uv pip install git+https://github.com/lkm2835/vllm.git@add-exaone4_5
uv pip install git+https://github.com/nuxlear/transformers.git@add-exaone4_5
```

After you install the vLLM, you can launch the server with the following code snippet. You can remove unnecessary arguments from the snippet.

```bash
vllm serve LGAI-EXAONE/EXAONE-4.5-33B \
    --served-model-name EXAONE-4.5-33B \
    --port 8000 \
    --tensor-parallel-size 2 \
    --max-model-len 262144 \
    --reasoning-parser qwen3 \
    --enable-auto-tool-choice \
    --tool-call-parser hermes \
    --limit-mm-per-prompt '{"image": 64}' \
    --speculative_config '{
        "method": "mtp", 
        "num_speculative_tokens": 3
    }'

```

An OpenAI-compatible API server will be available at http://localhost:8000/v1.


### SGLang

Both Transformers and SGLang of our forks are required to utilize EXAONE 4.5 model. 
You can install the requirements by running the following commands:

```bash
uv pip install git+https://github.com/lkm2835/sglang.git@add-exaone4_5
uv pip install git+https://github.com/nuxlear/transformers.git@add-exaone4_5
```

After you install the SGLang, you can launch the server with the following code snippet. You can remove unnecessary arguments from the snippet.

```bash
python -m sglang.launch_server \
    --model-path LGAI-EXAONE/EXAONE-4.5-33B \
    --served-model-name EXAONE-4.5-33B \
    --port 8000 \
    --tp-size 2 \
    --mem-frac 0.81 \
    --reasoning-parser qwen3 \
    --tool-call-parser hermes \
    --speculative-algorithm EAGLE \
    --speculative-num-steps 3 \
    --speculative-eagle-topk 1 \
    --speculative-num-draft-tokens 4

```

An OpenAI-compatible API server will be available at http://localhost:8000/v1.


### llama.cpp

You should build the llama.cpp from [our fork](https://github.com/nuxlear/llama.cpp/tree/add-exaone4_5). Please refer to [the guide](https://github.com/ggml-org/llama.cpp/blob/master/docs/build.md) from the original repository.

After you build the llama.cpp library, you can launch the server with the following code snippet. You can remove unnecessary arguments from the snippet.

```bash
llama-server \
    -m EXAONE-4.5-33B-Q4_K_M.gguf \
    -mm mmproj-EXAONE-4.5-33B-BF16.gguf \
    -ngl 999 -cb \
    -c 262144 -n 32768 \
    -fa on -sm row \
    --temp 1.0 --top-p 0.95 --min-p 0 \
    --presence-penalty 1.5 \
    --no-context-shift \
    --port 8000 \
    -a EXAONE-4.5-33B \
    --jinja
```

When the server is ready, you can test the model using the chat-style UI at http://localhost:8000, and access the OpenAI-compatible API at http://localhost:8000/v1.



### Using EXAONE 4.5

After launching the OpenAI-compatible server with EXAONE 4.5, you can seamlessly use the model via API with a single code integration, even though the serving framework has changed. To use OpenAI Python SDK and following examples, you should install the `openai` library on your environment.


> [!IMPORTANT]
> To achieve the expected performance, we recommend using the following configurations:
> - We recommend to use `temperature=1.0`, `top_p=0.95`, `presence_penalty=1.5` for general purpose.
> - We recommend to use `temperature=0.6`, `top_p=0.95`, `presence_penalty=1.5`, `top_k=20` for OCR/document-related tasks, and Korean inputs.
> - We recommend to use `temperature=1.0`, `top_p=0.95` for text-only inputs.
> - Different from EXAONE-4.0, EXAONE 4.5 uses `enable_thinking=True` as default. Thus, you need to set `enable_thinking=False` when you want to use non-reasoning mode.
> - EXAONE 4.5 prefers using `\boxed{}` format to answer the question. We recommend using this format with the corresponding format instruction for better parsing accuracy. 
>



You can easily try model's chat completions by using OpenAI Python SDK. For your server in local machine, you will need to change your `base_url` and `api_key` for the OpenAI client.


### Image-Text QA

#### Reasoning mode

For tasks that require accurate results, you can run the EXAONE 4.5 model in reasoning mode as follows.

```python
from openai import OpenAI

client = OpenAI(
    base_url="http://localhost:8000/v1",
    api_key="EMPTY",
)

messages = [
    {
        "role": "user",
        "content": [
            {
                "type": "image_url",
                "image_url": {
                    "url": "https://github.com/Aim-Highest/EXAONE-4.5/blob/main/assets/exaone45_input2.png?raw=true",
                },
            },
            {
                "type": "text",
                "text": "How much larger is the model released in winter 2025 compared with the one released in summer 2024?",
            },
        ]
    }
]

response = client.chat.completions.create(
    model="EXAONE-4.5-33B",
    messages=messages,
    max_tokens=32768,
    temperature=1.0,
    top_p=0.95,
    presence_penalty=1.5,
    extra_body={
        "chat_template_kwargs": {
            "enable_thinking": True,  # default: True
        }
    }, 
)
print(response)
```

#### Non-reasoning mode

For tasks where latency matters more than accuracy, you can run the EXAONE 4.5 model in non-reasoning mode as follows.

```python
from openai import OpenAI

client = OpenAI(
    base_url="http://localhost:8000/v1",
    api_key="EMPTY",
)

messages = [
    {
        "role": "user",
        "content": [
            {
                "type": "image_url",
                "image_url": {
                    "url": "https://github.com/Aim-Highest/EXAONE-4.5/blob/main/assets/exaone45_input1.jpg?raw=true",
                },
            },
            {
                "type": "text",
                "text": "What dish is the person preparing, and how is it made?",
            },
        ]
    }
]

response = client.chat.completions.create(
    model="EXAONE-4.5-33B",
    messages=messages,
    max_tokens=32768,
    temperature=1.0,
    top_p=0.95,
    presence_penalty=1.5,
    extra_body={
        "chat_template_kwargs": {
            "enable_thinking": False,  # default: True
        }
    }, 
)
print(response)

```


### Text-only QA

```python
from openai import OpenAI

client = OpenAI(
    base_url="http://localhost:8000/v1",
    api_key="EMPTY",
)

messages = [
    {
        "role": "user",
        "content": "Explain how useful you are.",
    }
]

response = client.chat.completions.create(
    model="EXAONE-4.5-33B",
    messages=messages,
    max_tokens=32768,
    temperature=1.0,
    top_p=0.95,
    extra_body={
        "chat_template_kwargs": {
            "enable_thinking": True,  # default: True
        }
    }, 
)
print(response)

```


### Agentic Use

The following example demonstrates the agentic capability of EXAONE 4.5 for image-text inputs. You can use your own agents, skills, or other harnesses with the EXAONE 4.5 model.

```python
# If needed:
# pip install langchain langchain-openai langchain-mcp-adapters
# curl -LsSf https://astral.sh/uv/install.sh | sh
# sudo apt-get update && sudo apt-get install -y nodejs npm

import os
import asyncio
from langchain_openai import ChatOpenAI
from langchain.agents import create_agent
from langchain_mcp_adapters.client import MultiServerMCPClient

def print_message(msg):
    parts = msg.content if isinstance(msg.content, list) else [{"type": "text", "text": msg.content or ""}]
    text_out, reasoning_out = [], []

    for p in parts:
        if isinstance(p, dict):
            if p.get("type") in ("text", "output_text") and p.get("text"):
                text_out.append(p["text"])
            elif p.get("type") in ("reasoning", "reasoning_text") and p.get("text"):
                reasoning_out.append(p["text"])

    if reasoning_out:
        print("\n[assistant_reasoning_content]")
        print("\n".join(reasoning_out))
    if text_out:
        print("\n[assistant_content]")
        print("\n".join(text_out))

async def main():
    model = ChatOpenAI(
        model="EXAONE-4.5-33B",
        base_url="http://localhost:8000/v1",
        api_key="EMPTY",
        temperature=1.0,
        model_kwargs={"top_p": 0.95},
    )

    client = MultiServerMCPClient({
        "filesystem": {
            "transport": "stdio",
            "command": "npx",
            "args": ["-y", "@modelcontextprotocol/server-filesystem", "/tmp"],
        },
        "fetch": {
            "transport": "stdio",
            "command": "uvx",
            "args": ["mcp-server-fetch"],
        },
        "duckduckgo": {
            "transport": "stdio",
            "command": "uvx",
            "args": ["duckduckgo-mcp-server"],
        },
    })

    agent = create_agent(model, await client.get_tools())

    inputs = {
        "messages": [{
            "role": "user",
            "content": [
                {
                    "type": "text",
                    "text": (
                        "Look at the image and identify the landmark. "
                        "Use the DuckDuckGo MCP tool to verify its name, height, and location. "
                        "Then use the fetch tool to read a fuller article page about it. "
                        "Create /tmp/mcp-demo and write a short markdown file to "
                        "/tmp/mcp-demo/landmark.md with: name, location, height, and a one-sentence summary of the article. "
                        "Finally, return only the exact file content."
                    ),
                },
                {
                    "type": "image_url",
                    "image_url": {
                        "url": "https://upload.wikimedia.org/wikipedia/commons/a/a8/Tour_Eiffel_Wikimedia_Commons.jpg"
                    },
                },
            ],
        }]
    }

    async for step in agent.astream(inputs, stream_mode="values"):
        msg = step["messages"][-1]
        if getattr(msg, "type", "") == "ai":
            print_message(msg)
            for tc in getattr(msg, "tool_calls", []) or []:
                print(f"\n[tool call] {tc['name']}({tc['args']})")

if __name__ == "__main__":
    asyncio.run(main())

```





## Limitation

EXAONE 4.5 models, like all existing multimodal models, have certain limitations and may occasionally generate
inappropriate responses. The multimodal model generates responses based on the output probability of tokens, and it
is determined during learning from training data. While we make every effort to exclude personal, harmful, and biased
information from the training data, some problematic content may still be included, potentially leading to undesirable
responses. Please note that the text generated by EXAONE 4.5 models does not reflect the views of LG AI Research.

- Inappropriate answers may be generated, which contain personal, harmful or other inappropriate information.
- Biased responses may be generated, which are associated with age, gender, race, and so on.
- The generated responses rely heavily on statistics from the training data, which can result in the generation of
semantically or syntactically incorrect sentences.
- Since the models do not reflect the latest information, the responses may be false or contradictory.

LG AI Research strives to reduce potential risks that may arise from EXAONE 4.5 models. Users are not allowed to
engage in any malicious activities (e.g., keying in illegal information) that may induce the creation of inappropriate
outputs violating LG AI’s ethical principles when using EXAONE 4.5 models.



## License

The model is licensed under [EXAONE AI Model License Agreement 1.2 - NC](./LICENSE)



## Citation

```
@article{exaone-4.5,
  title={EXAONE 4.5 Technical Report},
  author={{LG AI Research}},
  journal={arXiv preprint arXiv:2604.08644},
  year={2026}
}
```


## Contact

LG AI Research Technical Support: contact_us@lgresearch.ai

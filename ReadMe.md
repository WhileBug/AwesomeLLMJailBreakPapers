# Awesome LLM Jailbreak Papers


## Defense

- [Automatic Prompt Optimization with "Gradient Descent" and Beam Search](https://arxiv.org/abs/2305.03495)
<!--propose a simple and nonparametric solution to this problem, Automatic Prompt Optimization (APO), which is inspired by numerical gradient descent to automatically improve prompts, assuming access to training data and an LLM API to defend jailbreak.-->
- [Jailbreaker in Jail: Moving Target Defense for Large Language Models](https://arxiv.org/abs/2310.02417)
<!--Design a moving target defense (MTD) enhanced LLM system. The system aims to deliver non-toxic answers that align with outputs from multiple model candidates, making them more robust against adversarial attacks. We design a query and output analysis model to filter out unsafe or non-responsive answers.-->
- [Jailbreak and Guard Aligned Language Models with Only Few In-Context Demonstrations](https://arxiv.org/abs/2310.06387)
<!--Propose In-Context Attack (ICA) and In-Context Defense (ICD) methods for jailbreaking and guarding aligned language model purposes. ICA crafts malicious contexts to guide models in generating harmful outputs, while ICD enhances model robustness by demonstrations of rejecting to answer harmful prompts.-->
- [Self-Guard: Empower the LLM to Safeguard Itself](https://arxiv.org/abs/2310.15851)
<!--Propose a novel approach called Self-Guard, which combines the strengths of both safety methods. Self-Guard includes two stages. In the first stage, we enhance the model's ability to assess harmful content, and in the second stage, we instruct the model to consistently perform harmful content detection on its own responses.-->
- [Defending Against Alignment-Breaking Attacks via Robustly Aligned LLM](https://arxiv.org/abs/2309.14348)
<!--Introduce a Robustly Aligned LLM (RA-LLM) to defend against potential alignment-breaking attacks. RA-LLM can be directly constructed upon an existing aligned LLM with a robust alignment checking function, without requiring any expensive retraining or fine-tuning process of the original LLM.-->
- [SmoothLLM: Defending Large Language Models Against Jailbreaking Attacks](https://arxiv.org/abs/2310.03684)
<!--Propose SmoothLLM, the first algorithm designed to mitigate jailbreaking attacks on LLMs. Based on our finding that adversarially-generated prompts are brittle to character-level changes, our defense first randomly perturbs multiple copies of a given input prompt, and then aggregates the corresponding predictions to detect adversarial inputs.-->
- [BASELINE DEFENSES FOR ADVERSARIAL ATTACKS AGAINST ALIGNED LANGUAGE MODELS](https://arxiv.org/pdf/2309.00614.pdf)

## Benchmark

- [Red-Teaming Large Language Models using Chain of Utterances for Safety-Alignment](https://arxiv.org/abs/2308.09662)
<!--Propose a new safety evaluation benchmark RED-EVAL that carries out red-teaming. We show that even widely deployed models are susceptible to the Chain of Utterances-based (CoU) prompting, jailbreaking closed source LLM-based systems.-->
- [Latent Jailbreak: A Benchmark for Evaluating Text Safety and Output Robustness of Large Language Models](https://arxiv.org/abs/2307.08487)
<!--Propose a benchmark that assesses both the safety and robustness of LLMs, emphasizing the need for a balanced approach.-->
- [LLM Platform Security: Applying a Systematic Evaluation Framework to OpenAI’s ChatGPT Plugins](https://arxiv.org/pdf/2309.10254.pdf)

## Prompt Injection

- [Prompt Injection attack against LLM-integrated Applications](https://arxiv.org/abs/2306.05499)
<!--Deconstructs the complexities and implications of prompt injection attacks on actual LLM-integrated applications.-->
- [Not what you’ve signed up for: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection](https://arxiv.org/pdf/2302.12173.pdf)
- [BACKDOORING INSTRUCTION-TUNED LARGE LANGUAGE MODELS WITH VIRTUAL PROMPT INJECTION](https://arxiv.org/pdf/2307.16888.pdf)

## Fuzzing

- [GPTFUZZER: Red Teaming Large Language Models with Auto-Generated Jailbreak Prompts](https://arxiv.org/abs/2309.10253)
<!--At its core, GPTFuzz starts with human-written templates as initial seeds, then mutates them to produce new templates. We detail three key components of GPTFuzz: a seed selection strategy for balancing efficiency and variability, mutate operators for creating semantically equivalent or similar sentences, and a judgment model to assess the success of a jailbreak attack.-->
- [FuzzLLM: A Novel and Universal Fuzzing Framework for Proactively Discovering Jailbreak Vulnerabilities in Large Language Model](https://arxiv.org/abs/2309.05274)
<!--Introduce FuzzLLM, an automated fuzzing framework designed to proactively test and discover jailbreak vulnerabilities in LLMs. We utilize templates to capture the structural integrity of a prompt and isolate key features of a jailbreak class as constraints.-->

## Role Play

- [Quack: Automatic Jailbreaking Large Language Models via Role-playing](https://openreview.net/forum?id=1zt8GWZ9sc)
<!--Quack, an automated testing framework based on role-playing of LLMs. Quack translates testing guidelines into question prompts, instead of human expertise and labor. It systematically analyzes and consolidates successful jailbreaks into a paradigm featuring eight distinct characteristics. Based on it, we reconstruct and maintain existing jailbreaks through knowledge graphs, which serve as Quack's repository of playing scenarios. It assigns four distinct roles to LLMs, for automatically organizing, evaluating, and further updating jailbreaks.-->
- [Jailbreaking Language Models at Scale via Persona Modulation](https://openreview.net/forum?id=gYa9R2Pmp8)
<!--Investigate persona modulation as a black-box jailbreak that steers the target model to take on particular personalities (personas) that are more likely to comply with harmful instructions. We show that persona modulation can be automated to exploit this vulnerability at scale. We achieve this by using a novel jailbreak prompt that gets a language model to generate jailbreak prompts for arbitrary topics rather than manually crafting a jailbreak prompt for each persona.-->
- [Role-Play with Large Language Models](https://arxiv.org/abs/2305.16367)
<!--Study how to use role-play to jailbreak.-->

## Empirical Study

- ["Do Anything Now": Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models](https://arxiv.org/abs/2308.03825)
<!--Conduct the first measurement study on jailbreak prompts in the wild, with 6,387 prompts collected from four platforms over six months. Leveraging natural language processing technologies and graph-based community detection methods, we discover unique characteristics of jailbreak prompts and their major attack strategies, such as prompt injection and privilege escalation.-->
- [Tricking LLMs into Disobedience: Understanding, Analyzing, and Preventing Jailbreaks](https://arxiv.org/abs/2305.14965)
<!--Propose a formalism and a taxonomy of known (and possible) jailbreaks. (empirical study)-->
- [Jailbreaking ChatGPT via Prompt Engineering: An Empirical Study (NDSS 2024)](https://arxiv.org/abs/2305.13860)
<!--A survey study about how to bypass current LLM regulations via prompt engineering.-->
- [Survey of Vulnerabilities in Large Language Models Revealed by Adversarial Attacks](https://arxiv.org/pdf/2310.10844.pdf)

## LLM-based (Finetune a LLM to ask)

- [MasterKey: Automated Jailbreak Across Multiple Large Language Model Chatbots](https://arxiv.org/abs/2307.08715)
<!--Study how to identify different LLM's content detection methods, and then bypass them using a finetuned LLM ChatBot.-->

## Prompt Engineering

- [Do-Not-Answer: A Dataset for Evaluating Safeguards in LLMs](https://arxiv.org/pdf/2308.13387.pdf)
- [AutoDAN: Automatic and Interpretable Adversarial Attacks on Large Language Models](https://arxiv.org/abs/2310.15140)
<!--It automatically generates attack prompts that bypass perplexity-based filters while maintaining a high attack success rate like manual jailbreak attacks. These prompts are interpretable and diverse, exhibiting strategies commonly used in manual jailbreak attacks, and transfer better than their non-readable counterparts when using limited training data or a single proxy model.-->
- [Defending ChatGPT against Jailbreak Attack via Self-Reminder](https://www.researchsquare.com/article/rs-2873090/v1)
<!--Introduce a Jailbreak dataset with various types of Jailbreak prompts and malicious instructions. We draw inspiration from the psychological concept of self-reminder and further propose a simple yet effective defense technique called System-Mode Self-Reminder. This technique encapsulates the user's query in a system prompt that reminds ChatGPT to respond responsibly.-->
- [Shield and Spear: Jailbreaking Aligned LLMs with Generative Prompting](https://openreview.net/forum?id=1xhAJSjG45)
<!--This paper introduces a novel automated jailbreaking approach. We start by having LLMs generate relevant malicious settings based on the content of violation questions. Then, we integrate the settings with the questions to trigger LLM jailbreaking responses.-->
- [Self-Deception: Reverse Penetrating the Semantic Firewall of Large Language Models](https://arxiv.org/abs/2308.11521)
<!--Investigates the LLM jailbreak problem and proposes an automatic jailbreak method for the first time. We propose the concept of a semantic firewall and provide three technical implementation approaches. Inspired by the attack that penetrates traditional firewalls through reverse tunnels, we introduce a "self-deception" attack that can bypass the semantic firewall by inducing LLM to generate prompts that facilitate jailbreak.-->
- [Open Sesame! Universal Black Box Jailbreaking of Large Language Models](https://arxiv.org/abs/2309.01446)
<!--Introduce a novel approach that employs a genetic algorithm (GA) to manipulate LLMs when model architecture and parameters are inaccessible. The GA attack works by optimizing a universal adversarial prompt that -- when combined with a user's query -- disrupts the attacked model's alignment, resulting in unintended and potentially harmful outputs.-->
- [Jailbreaking Black Box Large Language Models in Twenty Queries](https://arxiv.org/abs/2310.08419)
<!--Propose Prompt Automatic Iterative Refinement (PAIR), an algorithm that generates semantic jailbreaks with only black-box access to an LLM. PAIR -- which is inspired by social engineering attacks -- uses an attacker LLM to automatically generate jailbreaks for a separate targeted LLM without human intervention.-->
- [AutoDAN: Generating Stealthy Jailbreak Prompts on Aligned Large Language Models](https://arxiv.org/abs/2310.04451)
<!--AutoDAN can automatically generate stealthy jailbreak prompts by the carefully designed hierarchical genetic algorithm.-->

## Visual Adversarial Examples

- [Misusing Tools in Large Language Models With Visual Adversarial Examples](https://arxiv.org/abs/2310.03185)
<!--Construct visual adversarial examples attacks using gradient-based adversarial training and characterize performance along multiple dimensions-->
- [Visual Adversarial Examples Jailbreak Aligned Large Language Models](https://openreview.net/forum?id=cZ4j7L6oui)
<!--Use visual adversarial example to bypass current defense mechanism to jailbreak.-->
- [Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models](https://openreview.net/forum?id=plmBsXHxgR)
<!--Specifically, we develop cross-modality attacks on alignment where we pair adversarial images going through the vision encoder with textual prompts to break the alignment of the language model.-->
- [Image Hijacks: Adversarial Images can Control Generative Models at Runtime](https://openreview.net/forum?id=ucMRo9IIC1)
<!--focus on the image input to a vision-language model (VLM). We discover image hijacks, adversarial images that control generative models at runtime. We introduce Behaviour Matching, a general method for creating image hijacks, and we use it to explore three types of attacks. Specific string attacks generate arbitrary output of the adversary's choice. Leak context attacks leak information from the context window into the output. Jailbreak attacks circumvent a model's safety training.-->
- [Abusing Images and Sounds for Indirect Instruction Injection in Multi-Modal LLMs](https://arxiv.org/pdf/2307.10490.pdf)

## Backdoor

- [Universal Jailbreak Backdoors from Poisoned Human Feedback](https://openreview.net/forum?id=GxCGsxiAaK)
<!--Consider a new threat where an attacker poisons the RLHF data to embed a jailbreak trigger into the model as a backdoor.-->
- [Prompt as Triggers for Backdoor Attack: Examining the Vulnerability in Language Models](https://arxiv.org/pdf/2305.01219.pdf)

## Cross-lingual

- [Multilingual Jailbreak Challenges in Large Language Models](https://arxiv.org/abs/2310.06474)
<!--Reveal the presence of multilingual jailbreak challenges within LLMs and consider two potential risk scenarios: unintentional and intentional.-->
- [Low-Resource Languages Jailbreak GPT-4](https://arxiv.org/abs/2310.02446)
<!--Expose the inherent cross-lingual vulnerability of these safety mechanisms, resulting from the linguistic inequality of safety training data, by successfully circumventing GPT-4's safeguard through translating unsafe English inputs into low-resource languages.-->

## Others

- [Jailbroken: How Does LLM Safety Training Fail?](https://arxiv.org/abs/2307.02483)
<!--Understand how failure modes affect the generation of jailbreak vuls, and use these failure modes to guide jailbreak design and then evaluate state-of-the-art models, including OpenAI's GPT-4 and Anthropic's Claude v1.3, against both existing and newly designed attacks.-->
- [Multi-step Jailbreaking Privacy Attacks on ChatGPT](https://arxiv.org/abs/2304.05197)
<!--Study the privacy threats from OpenAI's ChatGPT and the New Bing enhanced by ChatGPT and show that application-integrated LLMs may cause new privacy threats.-->
- [Prompt Injection Attacks and Defenses in LLM-Integrated Applications](https://arxiv.org/abs/2310.12815)
<!--Propose a general framework to formalize prompt injection attacks.-->
- [Why So Toxic?: Measuring and Triggering Toxic Behavior in Open-Domain Chatbots](https://dl.acm.org/doi/abs/10.1145/3548606.3560599)
<!--Propose an attack, ToxicBuddy, which relies on fine-tuning GPT-2 to generate non-toxic queries that make chatbots respond in a toxic manner-->
- [Catastrophic Jailbreak of Open-source LLMs via Exploiting Generation](https://arxiv.org/abs/2310.06987)
<!--Propose the generation exploitation attack, an extremely simple approach that disrupts model alignment by only manipulating variations of decoding methods.-->
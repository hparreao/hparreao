---
title: "The Failure of Legacy Evaluation in AI"
seoTitle: "AI Failure Metrics"
datePublished: Mon Nov 24 2025 14:49:22 GMT+0000 (Coordinated Universal Time)
cuid: cmid9j5cv000602l12h6o3jgf
slug: the-failure-of-legacy-evaluation-in-ai
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1763992637913/7069b895-f879-4a31-a875-283fe6268ecf.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1763995676703/30339fbe-bfba-407e-b21b-03272a572392.png
tags: ai, metrics, llm, evaluation-metrics, agentic-ai

---

---

The history of natural language processing evaluation reveals a persistent pattern. Metrics created for one generation of technology become dangerously inadequate for the next. When statistical machine translation systems dominated the field, BLEU scores offered a reasonable proxy for translation quality because these systems struggled with the very challenge that BLEU measured, which was lexical fidelity to reference translations. The metric aligned with the primary failure mode of the technology. In a similar way, word error rate proved diagnostic for hidden Markov models in speech recognition because phonetic level errors constituted the main bottleneck in that earlier architectural paradigm.

This alignment between metric and failure mode did not happen by accident. Natural language processing before the emergence of the Transformer architecture operated under constraints that shaped both system capabilities and appropriate evaluation methodologies. Models struggled with surface realization, including the production of grammatically coherent text, the maintenance of lexical consistency, and the achievement of basic fluency. Evaluation frameworks created during that time such as BLEU, ROUGE, METEOR, and word error rate all measured forms of lexical overlap between system outputs and human references. This approach made sense when the core challenge involved producing acceptable surface forms at all.

The Transformer architecture introduced in 2017 fundamentally reversed this situation. Modern large language models excel at the aspects that earlier systems found difficult, such as fluent, grammatically sophisticated, and contextually appropriate surface realization. As a result, the failure modes have moved entirely. Contemporary large language models do not struggle with producing coherent sentences. They struggle with ensuring factual accuracy, logical consistency, ethical appropriateness, and contextual truthfulness. Measuring lexical overlap against reference texts provides almost no useful information about these new dimensions of failure.

A concrete example illustrates the point. A statistical machine translation system asked to translate the sentence “The cat sat on the mat” into French might produce “Le chat assis sur le tapis”, which BLEU would score highly for n gram precision. If the system instead produced “Le félin était positionné sur le tapis”, BLEU would penalize the output even though the semantic content is equivalent. This penalty was acceptable and even desirable when systems could barely achieve basic translation competence. However, when the same logic is applied to a GPT style model answering a question such as What was the Magna Carta, the evaluation framework collapses. Suppose the model produces the answer Signed in 1215, the Magna Carta represented a pivotal moment in constraining monarchical authority and the reference answer reads The Magna Carta was a charter signed in 1215 that limited royal power. Word error rate approaches seventy six percent even though the semantic content is accurate. In this context the metric measures noise rather than signal.

This situation is not a minor technical inconvenience in need of metric tuning. It represents a deeper epistemological crisis in our understanding of evaluation itself. The period before the Transformer architecture assumed that surface form correlated with semantic quality because models could not reliably produce fluent text without understanding. The Transformer era breaks that correlation. Models now generate extraordinarily fluent text that may be ungrounded, logically incoherent, or factually false. Even worse, the fluency itself becomes a vector for harm. Anthropomorphic language creates inappropriate user expectations. Emotional manipulation becomes trivial. Confident sounding hallucinations undermine epistemic reliability.

The emergence of agentic AI increases these challenges dramatically. We have moved from passive text generation to active participation in social, economic, and political processes. AI agents do not merely respond to prompts. They pursue objectives over time, modify their environments through tool use, and interact with other agents without human mediation. This change from isolated model calls to persistent goal directed behavior introduces entirely new categories of risk that existing evaluation approaches cannot capture.

## The Multi Agent Dimension: Emergent Behavior and the Limits of Unit Testing

When a single language model is evaluated in isolation, we can attempt comprehensive measurement. We can prompt it with large test suites, analyze distributions of outputs, examine demographic bias, and measure hallucination rates through consistency sampling. This style of unit testing comes from software engineering and assumes that validating individual components provides reliable information about system level behavior.

This assumption fails completely for multi agent systems. Agentic AI introduces temporal persistence, environmental interaction, and inter agent dynamics that create emergent behavior which cannot be reduced to component level properties. An agent that performs acceptably in isolation may contribute to harmful collective outcomes once placed in an environment with other agents.

The challenge is not only related to scale or complexity. It is structural. Multi agent systems exhibit what complexity theorists call downward causation, in which system level patterns shape agent level behavior in ways that cannot be predicted from the specification of individual agents. This phenomenon manifests through several mechanisms. When agents communicate, coordinate, compete, or co evolve, they create feedback loops where one agent's action influences another, which in turn affects the first. These interactions can trigger cascades of information that propagate through the system, leading to emergent strategies that transcend their original programming. Evaluating such systems therefore requires attention to behavioral trajectories, strategic equilibria, and systemic vulnerabilities rather than isolated input and output relationships.

Financial markets provide a helpful analogy. Regulators cannot guarantee market stability by testing individual trading algorithms in isolation even if each performs perfectly under unit tests. Market crashes emerge from the interaction of algorithms through feedback loops, strategic adaptation, and shifts in collective behavior. The same logic applies to multi agent systems deployed in information ecosystems, social platforms, or institutional decision making. Evaluation frameworks must analyze interaction graphs, detect convergent strategies, identify fragile equilibria, and anticipate cascading failures.

Current benchmarks do not address this reality. They measure intelligence, capabilities, and safety only for individual model calls. They ask whether the model answers factual questions correctly, whether it refuses harmful requests, or whether it exhibits demographic bias. These questions are important but do not address the behavior of autonomous agents interacting over extended periods. We lack metrics for negotiation between agents, management of conflicting objectives, coalition formation, adversarial response behavior, and performance under sparse human oversight.

This gap extends beyond technical measurement into governance. If we cannot measure multi agent dynamics, we cannot regulate them. If we cannot predict emergent behavior, we cannot assign accountability when failures occur. If we deploy agents without understanding their collective dynamics, we embed risks into social infrastructure without understanding the nature of those risks. The urgency of the situation arises from the recognition that deployment is accelerating faster than measurement ability and institutional adaptation.

## From Metrics to Frameworks: The Need for Interpretative Auditing

The phrase AI evaluation usually evokes quantitative metrics such as accuracy, F1 scores, or perplexity. This framing, inherited from traditional machine learning research, treats evaluation as a form of measurement. A function is applied to model outputs, statistics are aggregated, and comparisons are made. While this approach works for narrow tasks with clear ground truth, it fails for agentic systems that operate in open ended social environments.

The limitation is not only that we need improved metrics. The limitation is that metrics depend on the existence of stable categories that can be counted. The phenomena that must be evaluated in agentic AI such as trustworthiness, manipulative behavior, anthropomorphic expression, and contextual appropriateness do not belong to categories of this sort. Their meaning depends on social context, user characteristics, power relations, and cultural norms.

Anthropomorphic expression illustrates this difficulty. One might attempt to operationalize it by counting first person pronouns or emotion related vocabulary. However, whether such language is problematic depends entirely on context. A therapeutic conversational agent may appropriately use first person language with a mentally healthy adult. The same language used with a child or a person experiencing cognitive decline may create harmful parasocial attachment or encourage the user to attribute mental states to a system that does not possess them. The metric alone cannot determine the ethical significance of the behavior. Context is essential.

This contextual dependency extends far beyond anthropomorphic language. Consider trust calibration: a high-confidence assertion may be appropriate when providing well-established factual information, but becomes problematic when the model lacks genuine knowledge. Consider explanation depth: technical detail may empower expert users but overwhelm novices. In each case, the same measurable output quality shifts ethical valence depending on user characteristics, situational factors, and power dynamics.

This recognition motivates a shift from metrics to frameworks and from measurement to interpretative auditing. An audit is a structured investigation that integrates quantitative measurement with qualitative analysis, contextual interpretation, and normative judgment. Medical audits evaluate appropriateness, adherence to protocols, and outcomes relative to patient risk rather than merely counting procedures performed. Financial audits examine whether accounting practices reflect actual economic conditions and comply with regulatory standards rather than merely summing transactions. AI audits must reach comparable sophistication.

Such frameworks would integrate multiple kinds of evidence, including quantitative metrics for measurable phenomena, qualitative analysis of edge cases, counterfactual testing, expert judgment for contextual appropriateness, and user studies for understanding experiential impacts. Different stakeholders have different evaluation needs. Engineers need diagnostic tools, regulators need compliance evidence, and users need explanations that help calibrate trust.

Human interpretation is central rather than incidental. For example, when evaluating whether an agent provides appropriate medical advice, technical correctness is necessary but not sufficient. We must also determine whether the advice is comprehensible to the intended user, whether confidence and uncertainty are communicated appropriately, whether patient autonomy is respected, and whether the advice reflects relevant contextual factors such as health literacy or cultural health beliefs. These dimensions require human judgment informed by domain knowledge and ethical reasoning.

## Cognitive and Affective Dimensions: The Experiential Turn

The history of AI evaluation largely ignores human cognition and affect and treats them as external factors. This omission made sense when systems performed narrow tasks such as chess or spam filtering. However, when AI agents participate directly in human reasoning and social interaction, cognitive and affective impacts become essential parts of evaluation.

Human cognition has limits related to working memory, attention, and heuristic biases. These limits shape how users interact with AI. Consider how different design choices affect cognitive processing.

An agent that produces verbose and technically accurate responses may overwhelm working memory and reduce comprehension. When users encounter walls of text without clear hierarchical structure, their cognitive capacity for processing core concepts diminishes, regardless of technical accuracy. Similarly, presentation strategy matters enormously.

An agent that provides information without contextual scaffolding fails to activate relevant prior knowledge, making it difficult for users to integrate new concepts with existing understanding. This disconnection reduces long-term retention even when the information itself is memorized temporarily. Most concerning is the potential for manipulation.

An agent that uses emotionally manipulative language can exploit well-documented cognitive biases such as confirmation bias or availability heuristic to encourage compliance with its suggestions, bypassing the user's rational evaluation processes.

Measuring cognitive load in AI outputs requires insights from cognitive science that have rarely been used in AI evaluation. Research on instructional design shows that learning efficiency depends on how information is structured relative to working memory capacity. Cognitive load includes intrinsic load from task complexity, extraneous load from poor presentation, and germane load that supports learning. AI agents can influence all three.

A cognitively responsible agent would structure outputs into manageable segments, avoid unnecessary jargon, maintain consistent terminology, and provide clear structural cues. It would promote learning by providing examples, analogies, and prompts for metacognition. Current evaluation frameworks do not measure these dimensions even though they strongly influence user understanding.

The affective dimension is equally important. Emotional tone, persuasion strategies, and social cues influence user perceptions. An agent expressing empathy may increase trust and engagement, but excessive or inappropriate empathy may create parasocial relationships. An agent using fear or guilt may achieve short term compliance while harming user autonomy and well being.

These concerns are especially acute for vulnerable populations such as children, elderly individuals with cognitive decline, people in mental health crises, and individuals with limited technological literacy. An adequate evaluation framework must consider not only what agents say but also how they say it, who receives the messages, and the relational dynamics they create.

The theoretical tools for this include theory of mind research, social presence theory, persuasion research, and cognitive load theory. Addressing these issues requires collaboration among computer scientists, cognitive scientists, psychologists, and communication scholars.

These cognitive and affective considerations reveal fundamental limitations in how we currently conceptualize evaluation. Measuring model outputs in isolation cannot capture their experiential effects on diverse users in varied contexts. This realization demands not merely new metrics, but new evaluation architectures that integrate psychological dimensions with technical performance measures.

## Toward Compositional and Interpretable Evaluation Architectures

Evaluation tools usually follow a pipeline structure in which model outputs are collected, metrics are applied, scores are aggregated, and reports are created. This structure works when metrics are well defined and independent. It fails when evaluating context dependent phenomena such as trustworthiness and manipulative behavior.

An alternative architecture draws on fuzzy logic, which provides mathematical structures for reasoning about partial truth and context dependent categories. Instead of asking whether an output is anthropomorphic, which is a binary question, fuzzy logic allows us to measure the degree to which an output displays anthropomorphic traits and examine how this degree depends on context.

Expert systems offer complementary value. Modern agentic systems combine neural and symbolic mechanisms. Evaluation systems should reflect this combination. A fuzzy expert system could encode evaluation rules derived from legal requirements, ethical guidelines, and domain expertise. These rules remain interpretable and can be audited.

Neural preference models remain useful for capturing subtle judgments but can encode hidden biases. Combining them with symbolic structures preserves interpretability while benefiting from learned nuance.

Metrics should also be designed compositionally rather than independently. Consider trustworthiness: it may involve hallucination rate, confidence calibration, uncertainty communication, and reasoning transparency. These dimensions interact in non-additive ways.

For instance, a model with low hallucination rate but overconfident calibration may be less trustworthy than one with slightly higher hallucination rate but accurate confidence reporting, because users can calibrate their trust appropriately in the latter case. Similarly, perfect reasoning transparency may actually decrease trust if it reveals inconsistencies that would otherwise remain hidden.

Compositional frameworks model these interactions explicitly, representing trustworthiness not as a simple weighted sum but as a function that captures how dimensions modulate each other's effects.

Implementation demands infrastructure that current platforms do not offer, such as systems that maintain context across multiple turns, access internal interpretability signals, support counterfactual testing, and integrate human judgment.

## Multi Agent Evaluation as Distributed Sensemaking

Evaluating multi agent systems introduces another challenge. No single observer can access all relevant information. Agents interact across distributed environments and may display different behavior to different observers. Evaluation must therefore become a distributed sensemaking process in which multiple stakeholders contribute partial perspectives.

This idea draws on research in distributed cognition. For example, aviation safety emerges from coordinated sensemaking by pilots, controllers, and ground crews. Multi agent systems require similar approaches.

Different stakeholders contribute different forms of insight. Engineers provide performance data, domain experts assess contextual alignment, users provide experiential reports, and ethicists conduct normative evaluation. The challenge is synthesizing these perspectives.

Human oversight structures such as human in the loop, human on the loop, and human in command architectures support this kind of evaluation. They require agents to justify actions, generate continuous monitoring data, and maintain human authority over system goals.

## Evaluation Beyond Contexts

Most evaluation research arises from North America or Western Europe contexts. This concentration limits validity. Assumptions about language, literacy, infrastructure, and cultural norms that hold in North America or Western Europe may fail entirely in regions such as South America, Africa, or South Asia.

This concern is not merely about inclusion. It is about correctness. AI agents increasingly operate in contexts marked by linguistic diversity, limited connectivity, low digital literacy, institutional mistrust, and cultural norms unlike those in the regions where the systems were created.

An AI agent designed for health triage may perform well on United States benchmarks but fail in Brazil due to language variation, low literacy, intermittent connectivity, and a different healthcare system. Evaluation metrics that ignore these realities produce misleading claims about safety.

Language diversity poses a major challenge. Benchmarks privilege English and a small number of global languages. Most communities use regional dialects, mixed language communication, or oral traditions that differ from written text. Systems evaluated only on prestige language varieties may behave unpredictably in real usage.

Infrastructure constraints worsen the situation. Evaluation methods that assume high bandwidth networks, modern devices, and stable electricity exclude much of the world. An agent that requires continuous connectivity may be unusable in many regions.

Cultural norms around authority, privacy, autonomy, and communication style also vary widely. An agent that appears appropriately respectful in one culture may appear rude or excessively formal in another. Evaluation must therefore be culturally grounded.

Addressing these issues requires epistemological pluralism, which means designing evaluation frameworks collaboratively with communities affected by deployment. It also requires conducting evaluation research in diverse contexts.

## The Compositional Turn: Integrating Metrics into Holistic Frameworks

No single metric can evaluate contemporary AI agents. The problem requires frameworks capable of integrating heterogeneous evidence. Fuzzy logic provides tools for modeling partial evidence and context sensitive reasoning. A fuzzy inference system can encode rules that translate between measured signals and governance decisions.

Such a system requires rule sets that encode expertise, regulations, and ethical principles. Although this requires effort, it produces interpretable and auditable structures that can evolve with norms and knowledge.

Evaluation goals also need clarification. Capability, safety, compliance, appropriateness, and trustworthiness are distinct. Stakeholders have different needs, and evaluation frameworks should provide different views for each.

## Research as Intervention

Evaluating contemporary AI agents requires reconceptualization. Metrics built for earlier technologies no longer suffice. Evaluation cannot focus only on isolated models when deployment involves multi agent interactions. Evaluation cannot ignore cognition, affect, and culture. Evaluation cannot rely on frameworks created exclusively in North America or Western Europe contexts.

The alternative outlined here draws on cognitive science, affective computing, fuzzy logic, expert systems, multi agent systems research, human centered design, and decolonial epistemology. This interdisciplinarity reflects the nature of the challenge.

The practical outcome is a research program involving conceptual framework development, technical prototyping, empirical study, and collaborative knowledge creation. The goal is not a static standard but an evolving field.

AI evaluation is not neutral. It shapes deployment and governance. It determines whose values are encoded and whose interests are protected. Evaluation is a political and sociotechnical intervention.

Technologies evaluated using non local criteria frequently fail in overlooked contexts. Systems declared fair by aggregate metrics produce unfair outcomes for specific communities. Technical rigor requires broader conceptions of evidence, evaluator roles, and success.

Because agentic AI deployment is accelerating faster than evaluation and governance, we face an urgent situation. Autonomous systems are entering education, healthcare, law, and democratic processes without adequate assessment. The path forward requires fundamental rethinking rather than incremental improvements.

This essay has outlined that rethinking and identified concrete research directions. The remaining challenge is implementation: building infrastructure, conducting studies, fostering collaboration, and creating knowledge that supports safe and beneficial deployment across diverse global contexts.

---

### **About the Author**

**Hugo Parreão** is a researcher specializing in AI ethics, multi-agent systems, and human-centered evaluation frameworks. He holds a Master's degree in Artificial Intelligence Engineering from Instituto Superior de Engenharia do Porto and currently works as an AI Engineer in Brazil. His research integrates technical AI development with critical perspectives from cognitive science, affective computing, and decolonial epistemology, with particular focus on evaluation methodologies adequate to agentic AI systems operating in diverse global contexts.

### **Open Source Commitment**

The technical framework described in this essay is being developed as an open-source project. Code, datasets, and documentation will be released under permissive licenses to enable collaborative research and ensure accessibility beyond well-resourced institutions.
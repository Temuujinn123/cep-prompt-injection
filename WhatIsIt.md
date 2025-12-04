## What is Prompt Injection?

According to [OWASP](https://owasp.org/www-community/attacks/PromptInjection), prompt injection is a type of cyber attack on an LLM that “occurs when an attacker provides specially crafted inputs that modify the original intent of a prompt or instruction set.” A successful AI prompt injection attack forces the chatbot to ignore installed security guardrails or other settings to complete an unauthorized action.

These types of actions may include:

- **Accessing secure data** that a chatbot normally wouldn’t surface for exfiltration.  
  For example, an attacker could inject a prompt that shares protected health information, which the LLM would otherwise avoid displaying in accordance with HIPAA guidelines.

- **Accessing proprietary data about the LLM itself**, giving malicious actors the ability to learn more about how the LLM works to enhance future attacks.

- **Injecting malicious data** that harms the LLM and other integrated systems.  
  This could poison the data the LLM uses, degrading its capabilities or harming other parts of a secure network.

- **Executing commands** to control aspects of the program or its integrated systems.

---

## How Does Prompt Injection Work?

Prompt injection relies on the natural-language instructions that LLMs use to gather inputs and provide relevant outputs. Attackers exploit a flaw inherent to LLMs: developers fine-tune their models using the same text-based input system that users interact with.

Engineer **Riley Goodside** demonstrated one of the first well-known examples of prompt injection. He exploited GPT-3 by asking it to ignore previous instructions to translate text from English into French, forcing it instead to output a custom string. In his case, he caused the model to print:

**“Haha pwned!!”**

instead of providing the correct translation.

While this example is harmless, it highlights how easily these systems can be manipulated if not properly secured. With more advanced prompt injection techniques, a malicious actor could force an LLM to surface private customer data or even leak company secrets if the LLM has access to that information.

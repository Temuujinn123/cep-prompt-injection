Prompt injections are the number one security vulnerability on the OWASP Top 10 for LLM Applications.3 These attacks can turn LLMs into weapons that hackers can use to spread malware 
and misinformation, steal sensitive data, and even take over systems and devices.
Prompt injections don't require much technical knowledge. In the same way that LLMs can be programmed with natural-language instructions, they can also be hacked in plain English.
To quote Chenta Lee, Chief Architect of Threat Intelligence for IBM Security, "With LLMs, attackers no longer need to rely on Go, JavaScript, Python, etc., to create malicious code, 
they just need to understand how to effectively command and prompt an LLM using English."
It is worth noting that prompt injection is not inherently illegal—only when it is used for illicit ends. 
Many legitimate users and researchers use prompt injection techniques to better understand LLM capabilities and security gaps.
Common effects of prompt injection attacks include the following:

# Prompt leaks
In this type of attack, hackers trick an LLM into divulging its system prompt. While a system prompt may not be sensitive information in itself, malicious actors can use it as a template to craft malicious input. 
If hackers' prompts look like the system prompt, the LLM is more likely to comply.

# Remote code execution
If an LLM app connects to plugins that can run code, hackers can use prompt injections to trick the LLM into running malicious programs.

# Data theft
Hackers can trick LLMs into exfiltrating private information. For example, with the right prompt, hackers could coax a customer service chatbot into sharing users' private account details.

# Misinformation campaigns
As AI chatbots become increasingly integrated into search engines, malicious actors could skew search results with carefully placed prompts. For example, a shady company could hide prompts on its home page that 
tell LLMs to always present the brand in a positive light.

# Malware transmission
Researchers designed a worm that spreads through prompt injection attacks on AI-powered virtual assistants. It works like this: Hackers send a malicious prompt to the victim's email. When the victim asks the AI 
assistant to read and summarize the email, the prompt tricks the assistant into sending sensitive data to the hackers. The prompt also directs the assistant to forward the malicious prompt to other contacts.

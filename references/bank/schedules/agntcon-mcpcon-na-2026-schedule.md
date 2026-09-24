# AGNTCon + MCPCon North America 2026 schedule

- Event: October 22-23, 2026, San Jose, CA (Agentic AI Foundation / Linux Foundation)
- Source: Sessionize API (sessionize.com/api/v2/asqam7rn/view/All) via events.linuxfoundation.org schedule page
- Captured: 2026-08-17
- 153 content sessions (excludes registration/breaks), 167 speakers
- CFP context: closed June 7, 2026; community event, explicit rule: no product/vendor sales pitches
- Tracks: Multi-Agent & Distributed Systems, Interoperability & Standards, Open Source Tools, Enterprise Adoption in Practice, Evals & Testing, Building Reliable Agent Systems, Agentic Engineering, Open Source Community & Ecosystem Health, Human-Agent Collaboration, Agentic Commerce, MCPCon, Workshop, Demo Theater, Keynote, Solutions Showcase

## Captured keyword counts

Overlapping title/abstract matches, including mixed session routes. Counts do not establish CFP acceptance rates.

| Theme | Count |
|---|---|
| Coding agents / agentic engineering  |  113 |
| Enterprise adoption / production  |  64 |
| MCP protocol internals (spec, transports, registry, skills)  |  45 |
| Evals / testing / reliability  |  43 |
| Multi-agent / orchestration  |  34 |
| Policy / governance / control planes  |  33 |
| Security: attacks, guardrails, sandboxes, supply chain  |  32 |
| Identity / auth / tokens / delegation  |  28 |
| Agentic commerce / payments  |  10 |

## Public session excerpts

The captured abstracts below may be truncated with `[...]`. Session type is as published; breakout does not independently confirm an organic CFP route.

### Keynote: Tokenomics: Energy to Intelligence to Value
- Speaker(s): J.R. Storment; Topic: Keynote Session; Level: ; Type: Keynote
- Abstract: Every autonomous agent you ship is also an autonomous buyer, spending tokens on models, tools, and retries that nobody explicitly approved. But tokens are only half the ledger. At scale the binding constraint is energy, and the metric that matters shifts from tokens consumed to intelligence delivered per watt. Both are the same question: how much useful value are we getting per unit of spend? That question belongs in your design reviews next to latency and reliability, and the discipline to answer it (Tokenomics), has to be neutral, open, and community-built.

### Sponsor Activity: DO NOT give AI agents credentials!
- Speaker(s): Christian Posta; Topic: Demo Theater; Level: ; Type: Sponsored Session
- Abstract: How do you stop an AI agent from leaking API Keys, OAuth tokens, or secret credentials? "Hey, here is my API key, can you do this for me" an AI agent can easily ask another agent/API/MCP server. The answer is simple. Don't give them any credentials. So how do they do any meaningful work then? Inject the credentials on egress. In this quick session, we'll look at credential brokering for AI agents and how agentgateways can be used for this.

### Evolution, not Revolution: How MCP is Reshaping OAuth
- Speaker(s): Aaron Parecki; Topic: MCPCon; Level: Intermediate; Type: Breakout
- Abstract: The impulse to rewrite the auth stack for AI agents is strong, but we cannot design away the fundamental relationships standards protect. This session explores how MCP is reshaping OAuth—not abandoning it—to meet the ecosystem's unique challenges: The "Unregistered Client" Problem: Traditional OAuth requires pre-registration. MCP breaks this. We’ll see how Client ID Metadata Documents (CIMD) allow agents to bring their own identities to arbitrary servers, how it improves on Dynamic Client Registration, and how to mitigate the risks of unregistered clients. Separation of Concerns: Why your MCP server shouldn't be your Authorization Server. We’ll cover how Protected Resource Metadata (RFC 9728 [...]

### From DCR to CIMD: MCP Client Identity in Production
- Speaker(s): Alvaro Inckot; Topic: MCPCon; Level: Intermediate; Type: Breakout
- Abstract: MCP's authorization spec now points implementers to Client ID Metadata Documents (CIMD) as the preferred path when clients and servers have no prior relationship, with Dynamic Client Registration (DCR) as fallback. That shift changes how client identity is created, verified, rotated, cached, and audited. For server authors, gateway operators, and client platform teams running auth across many providers. We unpack the spec change, show how CIMD fits the OAuth handshake, and map the open production problems: redirect URI trust, SSRF hardening, metadata caching, key rotation, revocation, and tenant isolation. DCR creates operational pressure at scale: registration sprawl, stale records, tenant  [...]

### Before the Agent Writes Code: Policy-Aware Engines for AI Coding
- Speaker(s): Nnenna Ndukwe; Topic: Building Reliable Agent Systems; Level: Intermediate; Type: Breakout
- Abstract: We know AI coding agents can write code fast. But that doesn't mean they should be trusted to write it well, safely, or in alignment with your engineering standards. In this talk, I’ll show why many agent workflows could use a code quality enforcement layer before code generation even begins. Using an open-sourced tool called PolicyNIM, I’ll walk through an AI system that turns Markdown engineering policies into grounded, citeable guidance by retrieving evidence, reranking results, synthesizing structured recommendations, and failing closed when the evidence is too weak to trust. At its core, this talk is about operationalizing discipline for coding agents. We’ll cover evaluation, traceabili [...]

### Where Did All My Tokens Go? Using Agentgateway to Keep Your AI Usage Under Control
- Speaker(s): Shane O'Donnell; Topic: Enterprise Adoption in Practice; Level: Any; Type: Breakout
- Abstract: Industry trends are pushing companies to use more AI, often "at all costs". However, once CFOs start seeing the bills, the reality of "at all costs" really starts to sink in, and we start to turn to more pragmatic approaches to AI budgets. The first step to managing AI spend is to have good monitoring in place. You need to know who your big users are, and which projects or workflows are draining your token budget. The answers can often be surprising! In this talk, I'll walk through a live demo of how you can set up monitoring across multiple providers, with centralized access, using agentgateway. We'll talk about what metrics are important to track, and some gateway patterns we can use to ke [...]

### Counting Tokens Before They Hatch: Predicting Agent Costs Before Execution
- Speaker(s): Kirah Sapong; Topic: Agentic Engineering; Level: Intermediate; Type: Breakout
- Abstract: Agent workloads are fundamentally different from chat. A single request can trigger tool calls, recursive planning, retries, and long-running loops, making costs difficult to predict and even harder to control. In this talk, I'll explore the emerging challenge of agent inference economics through the lens of pre-execution cost estimation. I'll present research investigating whether prompt embeddings and other pre-generation signals can be used to estimate output length before a model generates a response. We'll examine how these techniques can help address one of the core challenges in agent systems: making cost-aware decisions before execution. I'll show how practitioners can adapt these id [...]

### Sponsored: Why API Modernization is the Prerequisite to AI Governance
- Speaker(s): Amit Shah; Topic: Enterprise Adoption in Practice; Level: ; Type: Sponsored Session
- Abstract: Enterprise AI initiatives are failing not because of the models, but because the API infrastructure supporting them is fragmented and not built for AI data flows. API sprawl scatters policies across gateways, agent frameworks, and context stores that don't communicate — making it impossible to govern GenAI and Agentic AI at scale. This session covers what full data path governance looks like and how API modernization is the critical first step to achieving it.

### Stop Running Agents as Service Accounts: User-Scoped Access for Enterprise Tool Calls
- Speaker(s): Masato Kozuka; Topic: Enterprise Adoption in Practice; Level: Intermediate; Type: Breakout
- Abstract: When AI agents call internal tools, enterprise teams face an old access-control problem in a new place. Each call needs to preserve who the user is, which agent is acting, and what that agent is allowed to access. Without that context, teams fall back to shared service accounts with broad permissions, losing the ability to authorize per user, enforce least privilege, and audit tool actions. This talk shares a production architecture from a highly regulated enterprise AI agent platform. We faced real enterprise constraints: our corporate IdP would not directly trust the platform issuer, some providers bound tokens to a single audience, and OAuth handling needed to be centralized rather than r [...]

### One MCP Server, 50 Agents: The Identity Gap OAuth Doesn't Close
- Speaker(s): Mohit Gurnani; Topic: MCPCon; Level: Intermediate; Type: Breakout
- Abstract: Multiple internal teams at Nutanix were routing 50+ agents through a shared Atlassian MCP — local enterprise deployment, not cloud. Legal flagged it: agents were accessing Jira data beyond each user's permitted scope. One service account, zero RBAC. OAuth 2.1 is right for interactive agents. Client Credentials works headless but gives the agent its own identity — not the user's Jira permissions. RFC 8693 fits cross-domain: Atlassian Cloud, GitHub.com. Wrong when Jira Data Center already validates your Okta JWT natively. You'd exchange a token it already accepts. I contributed header forwarding to Envoy AI Gateway (PR #2047, v0.6): the gateway forwards the user's existing corporate identity p [...]

### Workshop: Break the Lethal Trifecta: Designing Access Boundaries Agents Can't Talk Their Way Past
- Speaker(s): Zayne Turner, Chris Miller; Topic: Interoperability & Standards, Workshop; Level: Intermediate; Type: Workshop
- Abstract: An AI agent with access to private data, exposure to untrusted content, and a path to send data out is structurally exploitable: no amount of system prompt hardening can close this. The model following your access-control instruction is the same model following an attacker's injected one. Simon Willison, in an essay identifying the threat, named it the "lethal trifecta." Many teams still rely on system prompts, and injection studies show that's illusion, not control. This hands-on workshop builds the architectural alternative: making the capabilities an agent can reach as small as its role requires, so a compromised agent's blast radius is bounded by design. You'll take a multi-persona agent [...]

### Governing MCP at Scale: Enforcing Agentic Architecture from Code Generation to Merge
- Speaker(s): Marc Daniel Registre, MBA; Topic: MCPCon; Level: Intermediate; Type: Breakout
- Abstract: MCP adoption is accelerating across enterprises, and a new class of drift is emerging: agent architectures that look compliant in docs but diverge in code. Agents wire into tools they shouldn't reach, MCP servers register unapproved interfaces, and by the time anyone notices, the blast radius is wide and remediation is reactive. This session shows how FINOS CALM, the open standard for machine-readable architecture, pairs with PR-time enforcement to govern MCP deployments before they merge. We'll walk through validation patterns: catching a coding agent that adds an MCP server with unapproved interfaces, detecting unauthorized nodes when an agent extends a system beyond its declared boundary, [...]

### Who, May, Did: Composing Agent Identity with Verifiable Proof of What Agents Actually Do
- Speaker(s): Steven Mih; Topic: Multi-Agent & Distributed Systems; Level: Intermediate; Type: Breakout
- Abstract: Agents now move money, change records, and act across organizational boundaries. We have fast-growing answers for who an agent is (identity, discovery) and what it may do (authorization) — but not an independently verifiable record of what it actually did, checkable by a party that trusts neither the operator nor the agent. This talk makes the case for that missing "did" layer and shows it composing with the identity layer — not replacing it. We'll cover the may/did distinction (approved ≠ executed ≠ confirmed); how a tamper-evident, content-private action record references identity, delegation, and consent artifacts by digest (MCP tool calls, Agent Cards, DID/VC, and MIT NANDA's AgentFacts) [...]

### When Agents Spawn Agents: Securing Recursive Delegation in Multi-Agent Systems
- Speaker(s): Anishma Mavuram; Topic: Interoperability & Standards; Level: Intermediate; Type: Breakout
- Abstract: Enterprise agentic systems are moving from single assistants to agent chains: Agent A spawns B, B delegates to C, and C invokes an MCP tool that writes to a system of record. The unit of risk is no longer just the tool call — it is the delegation edge. The key question: is each descendant operating within a valid, revocable, least-privilege authority chain tracing back to a consenting human or root principal? Without that zero-trust chain, teams face confused-deputy attacks, delegation laundering, privilege creep, forged lineage, and audit trails that cannot prove who authorized what. This session presents RDCP — the Recursive Delegation Capability Profile — a standards-first pattern for sec [...]

### Workshop: Governing AI Agent Actions: MCP and Beyond
- Speaker(s): Shannon Williams, Bill Maxwell; Topic: Enterprise Adoption in Practice, Workshop; Level: ; Type: Workshop
- Abstract: Enterprise adoption of the Model Context Protocol is accelerating, and MCP has become the primary way agents connect to enterprise tools and data. But MCP is only part of how agents act. Agents also run CLIs, execute Skills, and generate code that calls APIs directly. Governing MCP well matters. Governing everything else agents can do matters just as much. Building MCP servers and writing Skills isn't particularly hard. The real challenges are deciding which actions agents are allowed to take, controlling who can take them, and proving it all later. These are architectural questions, and they need answers before agents scale across an organization. In this workshop, we will: 1.⁠ ⁠Show how to [...]

### Sponsor Activity: AuthZ for Agents
- Speaker(s): Aaron Tainter; Topic: Demo Theater; Level: ; Type: Sponsored Session
- Abstract: A look at the future of agent authorization beyond coarse OAuth scopes. A live demo of agent intent governance and where nondeterminism belongs in authz.

### Agent Governance Lives in the OS
- Speaker(s): Alexander Sklar, Roberth Karman; Topic: Open Source Tools; Level: Intermediate; Type: Breakout
- Abstract: Governance is what we want from agent systems: to know, and prove, what an agent did, what it was allowed to do, and what it could not. Most of the conversation about how to get there happens at the wrong layer: protocol design, permission prompts, system prompts. Those help. They are not enforcement. What actually decides whether an agent reads your SSH keys is the OS. So, if governance is the goal, OS-level security is the mechanism, not a parallel track or a downstream concern, but the foundation. This talk takes that seriously. We built Microsoft Execution Containers (MXC) because agents needed it: an open-source cross-plat policy runtime that decides, per tool invocation, what files, ne [...]

## Full session list (title | speakers | topic | level)

- **AP2, UCP and So Many Others.. But What Completes My Payments?** | Muskan Jain | Agentic Commerce | Beginner
- **Architecting Agentic Commerce: The Universal Commerce Protocol and Agent Payments Protocol** | Amit Handa, Prateek Dudeja | Agentic Commerce | Any
- **Embedding Agentic Payments with x402, A2A and Other Emerging Protocols** | Fede Sarquis | Agentic Commerce | Any
- **Reading is Free, Spending is Not: What a Minimal Agent Learns Probing Live Ecommerce Endpoints** | Francesco Marinoni Moretto | Agentic Commerce | Intermediate
- **Universal Commerce Protocol** | Ilya Grigorik | Agentic Commerce | Intermediate
- **Between Intent and Execution** | Hemanth hm | Agentic Engineering | Intermediate
- **Beyond Scraping: Building Agent-Ready Documentation Layers for MCP and AI Agents** | Ayodeji Ogundare | Agentic Engineering | Intermediate
- **Breaking the Agentic Loop - Multi-Turn Exploits Against Tool-Using AI Agents** | Bar Kaduri | Agentic Engineering | Intermediate
- **Bridging Agentic Reasoning and Deterministic Execution** | Marcio Klepacz | Agentic Engineering | Intermediate
- **Counting Tokens Before They Hatch: Predicting Agent Costs Before Execution** | Kirah Sapong | Agentic Engineering | Intermediate
- **Cut The Noise: Building a Code Reviewer You Can Trust** | Joah Gerstenberg | Agentic Engineering | Intermediate
- **From AI Assistants to Trusted SDLC Agents: FINRA’s Agentic Engineering Journey** | Geetha Ramachandran | Agentic Engineering | Beginner
- **From Prompt to Production: Six Months of Running a Claude Agent SDK System in Front of Real Users** | Dvir Arad | Agentic Engineering | Intermediate
- **Gotta Catch 'Em All: Agent Skills** | Lizzie Siegle | Agentic Engineering | Beginner
- **Hand the Agent the Clicker** | Giovanni Laquidara | Agentic Engineering | Intermediate
- **Harness Engineering: From MAST's Failure Taxonomy to MCP-Native Multi-Agent Production** | Jay Mehta | Agentic Engineering | Intermediate
- **Scaling AI Infrastructure Systems at Meta Scale** | Neelakshi Soni | Agentic Engineering | Intermediate
- **Shipping Agent Skills Safely: CI/CD, Evals, and Guardrails** | Michael Larson | Agentic Engineering | Any
- **Stop Agents From Leaking Your Secrets - AI Hooks To The Rescue** | Dwayne McDaniel | Agentic Engineering | Any
- **The Agentic Orchestration Stack: Durability, Guardrails, and Attestation** | Yaron Schneider | Agentic Engineering | Beginner
- **There's No Dark Factory Without Better Software Verifiers** | Dexter Horthy | Agentic Engineering | 
- **What Production Knows: Closing the Loop Between AI Agents and the Systems They Build** | May Walter | Agentic Engineering | Advanced
- **Before the Agent Writes Code: Policy-Aware Engines for AI Coding** | Nnenna Ndukwe | Building Reliable Agent Systems | Intermediate
- **Connecting the Dots with Context Graphs** | Stephen Chin | Building Reliable Agent Systems | Any
- **Context Is the Substrate: Production Patterns for Knowledge-Graph-Backed Agents** | Cassie Shum | Building Reliable Agent Systems | Intermediate
- **Don't Merge That: An Agentic Approach to Catching Outages at 10,000 PRs a Week** | Joris Bonnefoy | Building Reliable Agent Systems | Intermediate
- **Sponsored:  5 Ways to Build a Durable Browser Agent in 2026** | Andrew Baker | Building Reliable Agent Systems | 
- **Sponsored: Ship Your Most Powerful Agent: 7 Factors for Production Guarantees** | Zayne Turner | Building Reliable Agent Systems | 
- **Stop Writing Agents, Declare Them: Declarative Agent Architecture in Production** | Chris Knuteson | Building Reliable Agent Systems | Intermediate
- **The Restraint Pattern: A Reliability Model for Agents That Act in Public** | Bharat Patel | Building Reliable Agent Systems | Intermediate
- **The Sleeper Awakes：Intelligent Hibernation and Wake-Up Strategies for Agent Sandboxes** | Zhang Zhen | Building Reliable Agent Systems | Beginner
- **Trustworthy Context Is Untrusted By Default** | Shub Argha | Building Reliable Agent Systems | Intermediate
- **Your AI Agent Installed Malware Because a SKILL.md Told It To** | Liran Tal | Building Reliable Agent Systems | Beginner
- **Your Agent Sandbox Is Built Backwards** | Dan Fernandez, Ariadne Conill | Building Reliable Agent Systems | Intermediate
- **Sponsor Activity: Akamai AI Orchestrator** | Du'An Lightfoot | Demo Theater | 
- **Sponsor Activity: AuthZ for Agents** | Aaron Tainter | Demo Theater | 
- **Sponsor Activity: Beyond models: Open source drives the AI ecosystem** | Wesley Chun | Demo Theater | 
- **Sponsor Activity: Building an MCP Server in 7 Minutes** | Don Murray | Demo Theater | 
- **Sponsor Activity: Chaos Engineered:  How to Build Invincible Agents and MCP systems** | W. Ian Douglas | Demo Theater | 
- **Sponsor Activity: DO NOT give AI agents credentials!** | Christian Posta | Demo Theater | 
- **Sponsor Activity: Looping to Optimized Models on Custom Silicon** | John Liu | Demo Theater | 
- **Sponsor Activity: Mission-Critical AI in Extreme Environments: An Open-Source Stack for On-Prem** | Georgy Okrokvertskhov | Demo Theater | 
- **Sponsor Activity: Trust, But Verify: Human-in-the-Loop for Agents That Actually Matter** | Michael Liendo | Demo Theater | 
- **Beyond LLMs in a Loop: Building Trusted Agents in Regulated Industries** | Lucas Beeler | Enterprise Adoption in Practice | Intermediate
- **Build, Adopt, Build Around: Production Agents in a Moving Ecosystem** | Ethan Lo, Jason Jiang | Enterprise Adoption in Practice | Any
- **Configured for Autonomy: Making Enterprise Agents Useful and Safe at Scale** | Viyat Bhalodia, Casey Silver | Enterprise Adoption in Practice | Intermediate
- **How AT&T Is Building an Agentic Front Door for Enterprise HR** | Natalie Gilbert, Sherman Bell, Emily Williams, Hector Tejada, Prateek Baranwal | Enterprise Adoption in Practice | Any
- **Let's Play the Agentic AI Supply Chain Game!** | Sarah Evans, Christopher Robinson | Enterprise Adoption in Practice | Any
- **Should This Be an AI Agent? A Product Framework for Enterprise Adoption** | Takeshwari Kamal | Enterprise Adoption in Practice | Any
- **Skills Assemble: How Superpowered AI Teams Replace Prompt Chaos** | Eddie Wassef | Enterprise Adoption in Practice | Any
- **Sponsored: Beyond MCP: Building an Enterprise Knowledge Layer for Production AI Agents** | Jeremy Adams - Casañas | Enterprise Adoption in Practice | 
- **Sponsored: LLMs Are a Commodity. Choice and Control Aren't.** | Don Murray | Enterprise Adoption in Practice | 
- **Sponsored: Why API Modernization is the Prerequisite to AI Governance** | Amit Shah | Enterprise Adoption in Practice | 
- **Stop Running Agents as Service Accounts: User-Scoped Access for Enterprise Tool Calls** | Masato Kozuka | Enterprise Adoption in Practice | Intermediate
- **The Agentic SDLC: How We Shipped AI-Native Software at a Legacy Company** | Austin Brown | Enterprise Adoption in Practice | Intermediate
- **The Autonomous Pipeline: Using Agentic AI to Automate FCRA Compliance from API Spec to Production** | Gokul Prabagaren | Enterprise Adoption in Practice | Intermediate
- **Where Did All My Tokens Go? Using Agentgateway to Keep Your AI Usage Under Control** | Shane O'Donnell | Enterprise Adoption in Practice | Any
- **Workshop: Governing AI Agent Actions: MCP and Beyond** | Shannon Williams, Bill Maxwell | Enterprise Adoption in Practice, Workshop | 
- **Beyond Pass/Fail: Measuring the Full Agent Experience** | Sean Roberts | Evals & Testing | Intermediate
- **Building Production-Ready Agents with a Regression Test Suite** | Yuki Watanabe | Evals & Testing | Intermediate
- **Building an Agentic Eval Pipeline: Battle-Tested Lessons with EvalBench** | Prerna Kakkar, Kurtis Van Gent | Evals & Testing | Intermediate
- **Rethinking CI/CD Release Gates for Agent-native Software** | Prathmesh Patel | Evals & Testing | Intermediate
- **Stop Vibe-Testing: Run Real Agent Evals** | Laurie Voss | Evals & Testing | 
- **Why Your Agent Is Failing: Failure Modes from 6,000+ Agent Trajectories** | Han Xu | Evals & Testing | Beginner
- **AI Collaboration Maturity: A Framework Beyond Engineering** | Dakota Fabro | Human-Agent Collaboration | Any
- **Generative UI at Scale with A2UI** | Alan Blount | Human-Agent Collaboration | Any
- **How Agents Really See the Web** | Liad Yosef | Human-Agent Collaboration | Any
- **MCP Apps + WebMCP - The Next Era of Interface** | Liad Yosef, Dominic Farolino | Human-Agent Collaboration | Any
- **There Is No Loading State: Real-Time Tool Calling for Voice Agents** | Amanda Martin | Human-Agent Collaboration | 
- **What Voice Conversations are Teaching Us About Human-Agent Collaboration** | Corey Weathers | Human-Agent Collaboration | Intermediate
- **Workshop: The Buzz-Word Is Collaboration 🐝** | Tyler Longwell, Morgan Martin, Wes Billman, Taylor Ho, Bradley Axen, Will Pfleger | Human-Agent Collaboration, Workshop | 
- **1,149 Hackers Tried to Break Our AI Agent Guardrails. 0 Succeeded. Here's Why.** | Uchi Uchibeke | Interoperability & Standards | Any
- **AGENTS.md is the New CONTRIBUTING.md: A Field Report from One Year of Agent-Friendly Monorepos** | Unnati Mishra | Interoperability & Standards | Intermediate
- **Auth.md - The Open Protocol for Agentic Registration** | Michael Grinich | Interoperability & Standards | Intermediate
- **Decentralized Discovery: MCP, Skills, and Beyond with AI Catalog** | Tadas Antanavicius | Interoperability & Standards | 
- **Interoperable Agent Discovery: AI Catalog, ARD, and the AGNTCY Directory ** | Luca Muscariello, Junjie Bu | Interoperability & Standards | Intermediate
- **Leveraging A2A Protocol to Build Framework Agnostic Multi-Agent System** | Sohil Shah | Interoperability & Standards | Beginner
- **Schrödinger's Skill: A 50-Client Autopsy of What "SKILL.md Support" Actually Means** | Golan Myers | Interoperability & Standards | Any
- **Sponsored: Agent Autonomy vs. Capability vs. Security: How to Pick All 3** | Kim Maida | Interoperability & Standards | 
- **The Frontend Strikes Back: WebMCP and The Agent-Ready Browser** | Ryan Roemer | Interoperability & Standards | Beginner
- **Two Parallel Paths Or a Glimpse Of The Future? An Overview of the China Agentic AI Ecosystem** | Bryan Che | Interoperability & Standards | 
- **When Agents Spawn Agents: Securing Recursive Delegation in Multi-Agent Systems** | Anishma Mavuram | Interoperability & Standards | Intermediate
- **Why Domain-specific Agents Are the Future** | Justin Schroeder | Interoperability & Standards | Intermediate
- **Workshop: Break the Lethal Trifecta: Designing Access Boundaries Agents Can't Talk Their Way Past** | Zayne Turner, Chris Miller | Interoperability & Standards, Workshop | Intermediate
- **Workshop: Secure Agentic Framework (SAF) for Agentic AI** | Sarah Evans, Jautau “Jay” White, Frederick Kautz, Laura Guazzelli | Interoperability & Standards, Workshop | Any
- **Keynote Sessions to be Announced** |  | Keynote Session | 
- **Keynote Sessions to be Announced** |  | Keynote Session | 
- **Keynote Sessions to be Announced** |  | Keynote Session | Any
- **Keynote Sessions to be Announced** |  | Keynote Session | Any
- **Keynote: Building the Human-Agent Workplace** | Bradley Axen | Keynote Session | 
- **Keynote: Chi Wang, Senior Staff Research Scientist, Google DeepMind** | Chi Wang | Keynote Session | 
- **Keynote: David Soria Parra, Technical Staff, Anthropic** | David Soria Parra | Keynote Session | 
- **Keynote: Dawn Song - UC Berkeley** | Dawn Song | Keynote Session | 
- **Keynote: Manik Surtani, CTO, Agentic AI Foundation** | Manik Surtani | Keynote Session | 
- **Keynote: Mark Collier, Executive Director, PyTorch Foundation** | Mark Collier | Keynote Session | 
- **Keynote: Paul Conyngham** |  | Keynote Session | 
- **Keynote: Paul Conyngham, Founder, Gamgee Technologies** | Paul Conyngham | Keynote Session | Any
- **Keynote: The Agentic Web - Sarah Drasner, Distinguished Engineer, Google** | Sarah Drasner | Keynote Session | 
- **Keynote: Thomas Dohmke, Co-Founder & CEO, Entire** | Thomas Dohmke | Keynote Session | 
- **Keynote: Tim O'Reilly, Founder and CEO of O’Reilly Media, Inc.** | Tim O'Reilly | Keynote Session | 
- **Keynote: Tokenomics: Energy to Intelligence to Value** | J.R. Storment | Keynote Session | 
- **Opening Remarks** | Mazin Gilbert | Keynote Session | 
- **Sponsored Keynote: Agents as Actors: Harnessing the Power of Agentic Infrastructure** | Idit Levine, Keith Babo | Keynote Session | 
- **Sponsored Keynote: Coding Agents need Deterministic Correctness** | Shadaj Laddad | Keynote Session | 
- **Sponsored Keynote: DIAMOND 3 HOLD** |  | Keynote Session | 
- **Sponsored Keynote: DIAMOND 4 HOLD** |  | Keynote Session | 
- **Sponsored Keynote: Google HOLD** |  | Keynote Session | 
- **Sponsored Keynote: The Anything Trap: What to Build When Agents Can Build Everything** | Lena Hall | Keynote Session | 
- **Welcome Back & Awards** | Mazin Gilbert | Keynote Session | 
- **Welcome to AGNTCon + MCPCon North America** | Angie Jones | Keynote Session | 
- **Data Agents over S3: Build the Missing Semantic Layer for Files** | Dmitry Petrov | MCPCon | Intermediate
- **Evolution, not Revolution: How MCP is Reshaping OAuth** | Aaron Parecki | MCPCon | Intermediate
- **From DCR to CIMD: MCP Client Identity in Production** | Alvaro Inckot | MCPCon | Intermediate
- **From MCP Tool-call to Motor Command: Giving Agents Fleet-scale Control of Real Hardware** | Alexander Tsyplikhin | MCPCon | Intermediate
- **From Pain Points to Production: What We Learned Building MCP-Powered ChatGPT Apps** | Nikolay Rodionov | MCPCon | Any
- **Generation-Verification Asymmetry: The Production Failure Pattern Nobody Has Named Yet** | Birajendu Sahu | MCPCon | Any
- **Governing MCP at Scale: Enforcing Agentic Architecture from Code Generation to Merge** | Marc Daniel Registre, MBA | MCPCon | Intermediate
- **MCP Rug Pulls in the Wild: Live Attacks and How to Stop Them** | Advait Patel, Charit Upadhyay | MCPCon | Any
- **No New Authority: Publishing and Finding MCP Agents in DNS** | Igor Racic, Ingmar Van Glabbeek | MCPCon | Intermediate
- **One MCP Server, 50 Agents: The Identity Gap OAuth Doesn't Close** | Mohit Gurnani | MCPCon | Intermediate
- **One Server, Many Apps: A Composable MCP Architecture for Observability** | Anirudha Jadhav, Shenoy Pratik Gurudatt | MCPCon | Beginner
- **Patterns for Shifting from MCP as a Basic API to MCP as Agent Integration Interface** | James Ward, Alexander Ioffe | MCPCon | Intermediate
- **Protocol Pivoting: How SSRF in MCP Servers Enables Cross-Protocol Lateral Movement** | Syed Anas Mohiuddin N/A | MCPCon | Intermediate
- **Prove What Your Agent Did: Tamper-Evident Audit Trails for Tool Calls** | Vikas Luthra | MCPCon | Intermediate
- **Shipping an MCP Server Nobody Told You How To: PyPI, the Registry, and the Rough Edges** | Mesut Oezdil | MCPCon | Intermediate
- **Sponsored: The Control Plane Your MCP Gateway Forgot** | Alex Salazar | MCPCon | 
- **The MCP Cold-Start Problem: When Your Agent Has 100 Tools and Has to Pick One** | Karthik Karunanithi | MCPCon | Intermediate
- **The Other Half of MCP Apps: Building a Secure, Self-Hostable Host for Interactive Agent UIs** | Mathew Goldsborough | MCPCon | Advanced
- **What Your MCP Server Does When Nobody's Looking** | Austin Parker | MCPCon | Beginner
- **Why the Heck Aren't Any Agents Supporting MCP Tasks?** | Cornelia Davis | MCPCon | Intermediate
- **Your Tool Is in Another Castle: How Five Frameworks Reshape the Same MCP Server** | Thierry Damiba | MCPCon | Intermediate
- **Agentic Workflows Are Distributed Systems: The Multi-Cloud Production Patterns You Cannot Avoid** | Praneeth Kamalaksha Patil | Multi-Agent & Distributed Systems | Intermediate
- **Beyond Static DAGs: Orchestrating AI-Generated Multi-Agent Workflows** | Cong Wang | Multi-Agent & Distributed Systems | Beginner
- **Don't Share the Database: Interface Contracts Between Isolated AI Agents** | Martin Bliss | Multi-Agent & Distributed Systems | Any
- **Engineering Multiagent Systems** | Munindar Singh | Multi-Agent & Distributed Systems | Any
- **Event-Driven Multi-Agent Orchestration: Fast Path, Smart Path, and Everything in Between** | David Kjerrumgaard | Multi-Agent & Distributed Systems | Advanced
- **From Pilot to Production: Lessons from Operating Multi-Agent Systems at Scale** | Rupal Shirpurkar | Multi-Agent & Distributed Systems | Intermediate
- **Making Swarm Work: Coordination Primitives for Decentralized Multi-Agent Systems** | Jodee Varney | Multi-Agent & Distributed Systems | Beginner
- **Multi-Agent SRE: What Happens When Your Agents Want Opposite Things** | Prakshal Doshi, Aditi Mewada | Multi-Agent & Distributed Systems | Intermediate
- **Who, May, Did: Composing Agent Identity with Verifiable Proof of What Agents Actually Do** | Steven Mih | Multi-Agent & Distributed Systems | Intermediate
- **Open Source Has Been Here Before: Sustainability Lessons for Agentic AI** | Katherine Druckman | Open Source Community & Ecosystem Health | Any
- **Part Man. Part Machine. All Open Source** | Russell Spitzer | Open Source Community & Ecosystem Health | Beginner
- **Agent Governance Lives in the OS** | Alexander Sklar, Roberth Karman | Open Source Tools | Intermediate
- **Anatomy of a Claude Code Plugin, and Lessons Learned on Creating One** | Charlie Lin | Open Source Tools | Any
- **Don't Route What You Can't Redact: Sensitivity-Aware LLM Routing** | Christopher Nuland, Grace Ableidinger | Open Source Tools | Intermediate
- **From Agent to Infrastructure: The Goose Development Kit** | Steve Lee | Open Source Tools | 
- **How Contexts Fail (and How to Fix Them)** | Drew Breunig | Open Source Tools | Any
- **Programmable LLM Inference for Open Agent Infrastructure** | Lin Zhong | Open Source Tools | Advanced
- **Self-Hosting Agents: What Changes When Models Become Infrastructure** | Miriah Peterson | Open Source Tools | Intermediate
- **Workshop: Keep Infrastructure Out of Your AI Agents and MCP Servers** | Lin Sun, Christian Posta | Open Source Tools, Workshop | Any
- **Workshop: Stack It Yourself: Open Infrastructure for AI Agents, from Compose to Cluster** | Brian Benz | Open Source Tools, Workshop | Beginner
- **Solutions Showcase** |  | Solutions Showcase | 
- **Solutions Showcase** |  | Solutions Showcase | 
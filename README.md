# Community Guidelines for Sustainability of Open-Source Ecosystem

Version 1.?, 2025-12-01

Copyright Naoki Shibata 2024-2025.

This document is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

&#127909; Watch the Official Introduction Video: [https://youtu.be/35zFfdCuBII](https://youtu.be/35zFfdCuBII)

## What is it?

These are non-binding community guidelines intended to be used as a code of conduct for OSS projects. The guidelines have the following features:

* **Remains entirely within the open-source framework:** It utilizes community norms rather than legal restrictions, ensuring it does not violate the Open Source Definition.
* **Aims to effectively exclude free-riders:** The explicit goal is to shut out corporate users who derive significant profits from the project's deliverables without bearing their share of maintenance costs.
* **Can be introduced anytime:** It can be adopted by any project at any stage, regardless of the specific distribution license being used. No relicensing is required.
* **Alleviates developer burnout:** It addresses the structural causes of sustainability issues.
* **Low burden on maintainers:** It is designed to be as objective as possible and avoids adding new management responsibilities to the project maintainer.

## How can I use it in my project?

To adopt this scheme, please copy the following files into your project repository:

1.  **[CODE_OF_CONDUCT.md](https://github.com/shibatch/nofreelunch?tab=coc-ov-file)**: Place this in the root directory.
2.  **[SUSTAINABILITY.md](https://github.com/shibatch/nofreelunch/blob/main/SUSTAINABILITY.md)**: Copy this directly into the product's README, immediately following the license notice, or place it in the root directory.
3.  **[CONTRIBUTING.md](https://github.com/shibatch/nofreelunch/blob/main/CONTRIBUTING.md)**: Place this in the root directory.
4.  **[PULL_REQUEST_TEMPLATE.md](https://github.com/shibatch/nofreelunch/blob/main/PULL_REQUEST_TEMPLATE.md)**: Place this in `.github` directory to be visible during Pull Requests.

It is distributed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## The Widening Gap Between FOSS Users and Maintainers

Today, it is commonplace for companies of all sizes to build their products and services on top of Free and Open Source Software (FOSS). Countless components that underpin modern business—databases, operating systems, compilers, encryption libraries, web frameworks—are published under FOSS licenses and can be deployed at virtually zero licensing cost.

However, at least some of this software is maintained by individual developers or small teams of volunteers, often in their spare time, with little to no financial compensation for the work required to keep the project secure, compatible, and reliable.

From the outside, FOSS may look like an inexhaustible public resource. Once code is released under a FOSS license, it can be copied and reused indefinitely at negligible cost. In reality, however, it is rare for the exact same version of code to remain usable over a long period without modification. Bug report triage, security vulnerability fixes, and adaptations to platform changes must be performed continuously, and these depend on human effort. Yet, currently, this effort is systematically unpaid, placing a burden on a small number of maintainers.

At the same time, many companies have built highly profitable products on top of this underfunded infrastructure. While they treat FOSS as a standard part of their technology stack, requests for support are often treated not as regular operating expenses, but as exceptional donations, or are not paid for at all. Many companies using FOSS do not treat FOSS maintainers as standard business partners.

As long as this gap exists—where FOSS is essential to business but there is little investment in the human talent that supports it—the FOSS ecosystem remains fragile. Popular projects receive a high volume of maintenance requests, but maintainers cannot respond to them unpaid indefinitely. 
User companies expect maintainers to provide professional service without paying them anything, but of course maintainers can't survive without pay and have other jobs. Why should maintainers be expected to provide such generous service only to companies that pay them nothing? Burnout and the sudden abandonment of projects become almost inevitable. Ultimately, the companies and users who have built upon these projects bear the risk.

The following sections explain this situation from a business risk perspective and demonstrate why a model that assumes endless free maintenance by upstream FOSS developers is not only unfair but structurally unsound as a business model.

#### A Broken Business Model Based on Unpaid Maintenance

Many companies adopt FOSS in their products as a prerequisite for their business continuity. This means that if the upstream project stops releasing security fixes or compatibility updates, these companies can no longer operate their products safely and reliably.

Nevertheless, a surprising number of organizations act as if they are entitled to unlimited free maintenance from upstream developers. They implicitly assume the following:

* The project will be continuously maintained.
* The company will continue to profit from it.
* There is no need to pay anything for the work that makes this possible.

If your business relies on software maintenance, but your business model assumes that maintainers will provide that maintenance for free forever, your business model is fundamentally flawed. You are simply shifting critical operating costs from your own balance sheet to the unpaid labor of others.

If companies truly desire business sustainability, it is only natural to protect the people and projects that support that business. In the case of FOSS, this means treating the developers who maintain critical dependencies as stakeholders, not as invisible, inexhaustible resources.

However, when asked to provide funds necessary for maintenance, such companies still respond with:

> "Why should we contribute when other companies aren't?"
>
> "Okay, we'll donate this time, but this is a special case."

Both responses are revealing.

* The first is a classic example of the **Tragedy of the Commons**. If everyone waits for "someone else" to pay for a public good, eventually no one pays, and the resource is depleted. The fact that others are free-riding does not make free-riding a rational or responsible choice.
* The second treats support for critical dependencies as an optional, exceptional act of charity, rather than a routine cost of business operations relying on those dependencies.

#### How Did We Get Here?

This situation did not arise because a specific company made a single wrong decision. It is the result of a series of individually reasonable choices accumulating into a structurally unsustainable pattern.

1.  **Adoption is easy and encouraged.**
    Engineering teams want to use attractive FOSS libraries and frameworks. Legal and compliance departments rarely have a clear reason to prohibit this. Licenses are widely adopted and generally do not impose direct payment obligations. Once the license is approved, the default answer is "Yes, you can use it."

2.  **Usage grows without built-in limits.**
    Once approved, there is usually no internal mechanism to limit the scope of FOSS usage. Engineers are encouraged to reuse proven components rather than reinventing the wheel. Over time, more and more products and services come to rely on the same set of FOSS projects, and some companies build highly profitable businesses based on them.

3.  **Maintenance costs are borne by the upstream project.**
    While the commercial value created by FOSS expands, the responsibility for maintenance remains with the original project. Upstream developers bear the cost of handling bug reports, security issues, and compatibility work, regardless of how much revenue downstream products generate.

4.  **Even if companies want to support FOSS, they face internal obstacles.**
    Many engineers within companies recognize that upstream projects need funding and want to support them. However, they run into several structural barriers:
    * **Donations are often practically difficult.** For large companies, direct donations to individuals or small groups are constrained by internal rules and external regulations (e.g., anti-corruption and anti-money laundering). Even if legally possible, internal audit and compliance processes can delay procedures and create bureaucracy.
    * **Funding other than donations comes with high legal overhead.** If a company provides financial aid through a contract rather than a donation, legal costs can be enormous. Each new contract requires review and negotiation, and internal processes are optimized for large vendors and clear deliverables, not suited for small upstream projects maintained by individuals.
    * **Standard contract templates are one-sided.** Many companies rely on "standard" procurement templates that assume suppliers will accept extensive warranties, strong indemnification, and in some cases, effectively unlimited liability or complete assignment of intellectual property. These terms might be negotiable with commercial vendors, but are completely unrealistic for individual maintainers. Yet, in reality, maintainers are often asked to sign exactly such terms if they want to receive any compensation.
    * **Non-monetary contributions are also difficult.** Code contributions to upstream can be politically sensitive within a company. Improvements that benefit all users, including competitors, may be viewed as strategically undesirable. In some organizations, internal policies explicitly prohibit engineers from creating code specifically for competitors, even when the company heavily relies on FOSS.
    * **Lack of empathy outside of engineering.** People in roles far removed from engineering (procurement, finance, middle management, etc.) often do not view FOSS developers as equal partners. Support for upstream projects is sometimes perceived as "charity" or a discretionary favor, and the amounts offered can be "pocket money" rather than a realistic budget for ongoing maintenance.

5.  **The means left to projects are extremely limited.**
    In this environment, it is difficult for a project to secure sustainable support simply by "expecting" companies to do the right thing. The only realistic option left is to clarify the project's expectations and make organizational free-riding visibly detrimental to a company's reputation. In other words, user companies need to realize that if they continue to deviate from the project's clear norms, it will eventually become difficult to continue using the FOSS product.

**Our position is simple:**

* If a revenue-generating product cannot function without maintaining a continuous dependency on FOSS, allocating a portion of that revenue to maintaining that dependency is not "generosity"—it is **basic risk management** and a normal operating expense.
* A company that refuses to fund the maintenance of dependencies essential to its business cannot be said to be running a sound, self-contained business. It is running a business that only functions as long as someone can be pressured or guilt-tripped into working for free.

We are not asking companies to "pay back for past benefits." We are asking them to take responsibility for the future of the infrastructure from which they profit today. If a business cannot survive without the continued unpaid labor of upstream FOSS developers, that business model is not just fragile; it is fundamentally unfair.

#### Our Scheme Overview

To address this situation, this project does not change software licenses or restrict users of the software. Instead, we use three complementary tools intended to work in concert:

* **`SUSTAINABILITY.md` / README Fragment**
    This statement explains the business risks of building products on unfunded Open Source Software (FOSS) and explicitly **requests** continuous financial support from organizations deriving more than a certain amount of annual revenue (currently US $1 million) from products using this project. It emphasizes that this is not a request for charity, but a proposal to treat maintenance as a regular operating expense and risk management measure, without affecting individual users or small-scale adopters.

    The sustainability statement is written as self-contained text but is designed to be copied directly into the product's README, immediately following the license notice. Many users do not read the project's code of conduct, perceiving it as "non-binding fine print." By placing the sustainability statement right after the license terms, everyone who needs to check the license conditions will also become aware of why commercial users' support is necessary for long-term maintenance.

* **`CONTRIBUTING.md` / Pull Request Template**
    For corporate contributors exceeding the same revenue threshold, we introduce a Corporate Contributor License Agreement (CCLA) that mirrors the aggressive contractual terms (such as unlimited liability and complete IP assignment) that some companies have tried to impose on this project in the past. The CCLA is intentionally crafted to highlight this asymmetry and to make it clear that if such terms are unacceptable to the company itself, they are also unacceptable when demanded of maintainers. Companies can receive an "Authorized Exemption" from the CCLA by entering into a separate, fair maintenance support agreement.

    This policy is designed to be visible in the contribution workflow. The project can include a shortened version of this policy and a checkbox in the Pull Request template. In this case, contributors are asked to confirm either: (a) their organization's revenue from products using this project is below the US $1 million threshold, (b) they agree to the CCLA, or (c) their organization has entered into a separate maintenance support agreement with the maintainers.

* **`CODE_OF_CONDUCT.md`**
    These guidelines define behavior that is desirable and undesirable from a sustainability perspective for project participants. We adopt the established "Code of Conduct" format not to give maintainers broad authority over people's private lives, but to visualize large-scale free-riding and provide a common language for members to question such behavior. These guidelines are non-binding and do not add legal conditions to the use of the software.

Given this design, a natural question arises: **Does such a scheme undermine the traditional strengths of FOSS?** The next section addresses this in detail.

#### Does this Code of Conduct Undermine the Strengths of FOSS?

We sometimes receive feedback asking, "Doesn't a code of conduct like this undermine the strengths of FOSS?" This is an important question that requires a careful answer.

When we talk about the "strengths of FOSS," we usually refer to points such as:
* The freedom to use the software for any purpose.
* Low friction in adoption (no lengthy negotiations or license servers required).
* The neutrality of software as shared infrastructure.
* The sense of a gift culture where participation is voluntary rather than transactional.

Our guidelines are designed not to weaken these strengths, but to protect them from a different, invisible threat: the expectation that while some developers provide unlimited free maintenance, other parties build massive, profitable businesses based on that work.

**1. Freedom of Use Remains Unchanged**
This project continues to be distributed under a true FOSS license. The license grants permission to use, modify, and redistribute the software. Our Code of Conduct does not impose legal conditions on the use of the software, nor does it alter the license terms.

The guidelines are non-binding. They prescribe behaviors considered desirable or undesirable for the long-term health of the project and the broader FOSS ecosystem; they do not define who is "allowed" to run the software in the first place.

If you wish to use this software without reading or agreeing to the guidelines, the license permits you to do so. The guidelines influence how your actions are perceived by others, not whether your use is legal.

What may be limited instead are the practical privileges associated with being treated as a responsible stakeholder in the project. This includes having maintenance and support requests taken seriously, the organization being welcomed as a community member, and the good reputation that comes with it. Companies that continue to free-ride despite clear expectations may face public recognition that their behavior is harmful to the project's sustainability. The license gives developers the technical freedom to use the code, but it does not grant unlimited rights to the maintainer's time, attention, or approval.

**2. The Real Threat to FOSS Freedom is Burnout and Hidden Obligations**
In reality, FOSS freedom is already being eroded—not by codes of conduct, but by hidden expectations of unpaid labor. We frequently hear statements from large companies like: *"We have customers, so you need to keep maintaining this. Our product depends on it."*

Often, this statement comes with a clear expectation that maintenance will be provided for free. This reverses the inherent responsibility. The company chose to build a commercial product on top of a dependency it neither funds nor controls. Even if that creates a business risk, it is a risk created by the company's own decision, not an obligation that magically appears on the maintainer's side.

If these expectations go unquestioned, maintainers are quietly treated as unpaid on-call staff for organizations that may be generating millions of dollars a year from products built on their work. Eventually, many maintainers burn out, and projects are abandoned. When that happens, "freedom of use" effectively becomes meaningless because there is no maintained software left to use.

Our guidelines make this hidden obligation visible and explicitly reject it. In effect, they argue: *"You are free to use the software. However, if you derive significant profit from the software, demanding unlimited free maintenance from the people who developed it is unfair and unsustainable."*

We believe this protects the true long-term freedom of FOSS: the freedom to rely on viable, maintained projects rather than abandoned code.

**3. Smooth Adoption is Maintained**
Another concern is whether prescriptive statements make FOSS adoption difficult in companies. Non-commercial licenses or mandatory support contracts certainly create friction, such as legal reviews, procurement approvals, and license servers.

Our guidelines explicitly avoid such models. We do **not** require:
* Prior negotiation before adoption.
* Purchase of license keys.
* Signing a support contract just to use the software.

Instead:
* Companies can adopt this software just like any other FOSS project.
* If annual revenue does not reach $1 million USD, no support is requested, and the manner of software use remains entirely unchanged.
* Even large enterprises can continue using the software exactly as before until they generate sufficient profits.
* Only when a company generates substantial revenue through this project will we request consideration for ongoing support. Even then, the specific support arrangements will be flexible and determined by the parties involved. No reporting on actual revenue generated is required.

In other words, while maintaining the "easy to try, easy to adopt" advantage of FOSS, we ask large commercial beneficiaries to treat sustainability as a normal operating expense, rather than a sudden emergency when maintainers eventually burn out.

**4. Neutrality of Use and Fairness to Maintainers**
Our guidelines do not prescribe *what the software is permitted to be used for*. We do not restrict fields of activity or police how businesses operate.

What we are discussing is how organizations treat FOSS maintainers and other contributors as stakeholders.
* Are they recognized as equal business partners in contract discussions?
* Can maintainers refuse terms (such as unlimited liability) that the company's own legal department would refuse to sign?
* If a product relies heavily on a maintainer's unpaid work, is there a willingness to share a portion of the revenue?

We also explicitly refuse to turn maintainers into judges of penalties.

#### Can This Scheme Change Corporate Awareness and Behavior?

Given all this, a natural question arises: Will companies truly understand that if they continue to deviate from the norms set by the project, it will eventually become difficult to keep using the FOSS product?

From a corporate perspective, continuing to use FOSS while facing criticism for free-riding carries a far more serious cost than the direct financial loss associated with contributing. When it becomes public knowledge that a company is extracting value from critical FOSS infrastructure without providing substantial support, it can be interpreted as a sign that the company condones unfair or myopic practices in its business operations.

In modern business, such perceptions have tangible consequences. Engineers and other highly skilled professionals carefully watch how companies treat the FOSS community when deciding where to work. For customers and partners, whether a vendor's behavior is sustainable and responsible is becoming an increasingly important evaluation criterion, alongside price and features. For public companies, institutional investors also assess reputational and operational risks arising fce on underfunded open-source projects. Therefore, being known as a company that systematically free-rides on FOSS is not just "bad PR"; it directly impacts hiring, retention, business negotiations, and ultimately, long-term corporate value.

Our guidelines leverage this reality. While they are not legally binding and do not change the terms of the software license, they clearly define behavior that is desirable and undesirable for the project and the broader FOSS ecosystem. By setting this standard, the guidelines allow anyone, including employees within the company, to point to a common public standard when questioning corporate behavior. Executives who choose to ignore the guidelines must explain—internally and externally—why their company continues to benefit from FOSS while refusing to meet expectations that many other organizations consider reasonable.

In this sense, the effectiveness of the guidelines comes from transparency and shared norms, not legal enforcement. When "using FOSS without contributing" is widely and clearly recognized as undesirable behavior, it becomes difficult for large, high-profile companies to continue such practices indefinitely without damaging their reputation. For many companies, the cost of being seen as a free-rider ultimately outweighs the cost of making an appropriate contribution. Our aim is not to punish companies with laws, but to create an environment where voluntary and active support for FOSS becomes the rational choice.

#### Crucial Benefit: Can be Introduced at Any Stage

One of the key features of this scheme is that it is built entirely on non-binding documents—the Code of Conduct and Sustainability Statement. Because these are not part of the software license and do not introduce new legal conditions on software use, projects can adopt them at any time, even after the software has been widely deployed and integrated into commercial products. No relicensing, no new click-through agreements, and no migration of existing users is required.

This has two important consequences:

* First, maintainers of existing projects retain the option to introduce this scheme when sustainability pressures become acute, without rewriting licenses or renegotiating terms with every user. The guidelines can be added as a layer of new, clear norms on top of the existing legal framework.
* Second, companies cannot reasonably assume that just because a project currently lacks such a code of conduct, it will remain norm-free forever. Maintainers may at any time adopt guidelines that clearly identify large-scale free-riding as undesirable and make that judgment visible. In such a scenario, companies that have profited from the project while refusing support must consider the risk that their behavior will later be publicly scrutinized, potentially leading to a loss of substantive access to the project community (e.g., inability to participate in issue tracking, discussions, or governance), even if the license itself does not change.

In other words, once such codes of conduct and sustainability statements exist and are easily adoptable, it is no longer safe for companies to build business models on the premise that upstream maintainers will provide endless free maintenance and never object. Smart organizations will treat support for critical FOSS dependencies as a standard part of risk management from the start, rather than waiting until a project formally adopts this framework and makes their existing behavior difficult to defend.

#### Designed to be License-Agnostic

Another key feature of this scheme is that it is independent of any specific software distribution license. The guidelines are intentionally separated from the license text and do not alter the permission terms of the software.

This means a project can adopt this Code of Conduct and associated sustainability scheme regardless of whether its current deliverables are distributed under GPLv3, MIT, Apache-2.0, BSD, or the public domain. No license change is required, and downstream users retain exactly the same legal rights as before. What changes is only the set of publicly stated expectations regarding how commercial beneficiaries are expected to act toward the project and its maintainers.

This license-agnostic nature allows the scheme to be introduced incrementally into many existing projects without forcing users to navigate a landscape of fragmented custom licenses. The legal freedom to use the software remains unified. The social expectation that major beneficiaries should help maintain their dependencies becomes a shared norm layered on top.

## Problems with existing codes of conduct

As the number of individuals from diverse backgrounds participating in open-source and free software projects continues to grow, an increasing number of such projects are adopting a code of conduct with the objective of ensuring that all participants have equal opportunity to contribute to the project.

A code of conduct is a set of rules that defines the normative behavior and responsibilities of individuals, parties, and groups. Typically, they are created for employees of a company in order to protect the company and to inform employees of the company's expectations. In general, codes of conduct in OSS projects state the following items:
* Respect and welcome diversity.
* Be patient, kind, do the best for the community, be considerate and cooperative.
* Condemn sexist/racist language, insults, jokes, violence or threats that harass marginalized people.
* Report unacceptable behavior to a specific group of team members who usually have the authority to determine appropriate action.

However, the issues addressed by these codes of conduct are not novel. Rather, they are long-standing concerns that have been present for some time, and these issues have been acknowledged and addressed to some extent. The recent emergence of these codes is perplexing. What prompted the introduction of these codes, and what are the benefits of having a code of conduct? What would be the consequences of not having one? There are numerous questions that remain unanswered.

In fact, there are OSS projects that oppose the introduction of such a code of conduct, and some strong opponents explicitly choose "No Code of Conduct" for their projects.

I have the following concerns in introducing a code of conduct to my project.

### Maintainers are not in a position to punish project members

The most important thing is that the basic human rights of each member are guaranteed. From the standpoint of guaranteeing freedom of speech, it is rather better not to have rules or anything like that restricting speech in non-project related venues. From a no-punishment-without-law standpoint, the project should not impose private penalties for offensive comments made by members on social networking sites that are not related to the project. Even if a member's non-project-related behavior has been found by an official agency to be illegal, whether the project should take any action in response is a matter for careful deliberation. It is the role of the authorities to punish members for illegal behavior, not the project maintainers, unless the authorities ask the maintainers to do something specific. The only thing that members of the project, including the maintainers, should do is to preserve evidence and to report any ongoing illegal activity related to the project to the public authorities.

Even if the code of conduct can restrict some actions of members, it is only on the web pages related to the project. The mere maintainers of an OSS project do not have the authority to tell project participants what to or not to say on social networking sites unrelated to the project. 

Banning a member in a project should be done out of necessity in order to defend the project, not to punish the member. Maintainers are not there to punish members. The idea of secretly telling the maintainer about the victimization and asking the maintainer to resolve it seems terribly childish. Maintainers are not the parents of the project members.


### Maintainers are not experts in resolving disputes between individuals

The resolution of disputes between individuals is often a very sensitive matter. It is a difficult task just to simply make factual determinations in cases of suspected illegal activity, and OSS project maintainers are typically not trained to do such things.

When the person alleging victimization secretly consults with the maintainer, it is often not easy for the maintainer to respond to that consultation. For example, if the claim of victimization is not valid, the maintainer needs to convince the consulter of this. In this process, if the maintainer inadvertently chooses wrong words, or even if everything is handled properly, the maintainer could also be accused of being a perpetrator.

Professional expertise is required in some cases to provide appropriate consultation, such as when the consulter suffers from a mental illness. It is not easy for an untrained maintainer to notice the mental illness, but the maintainer may still need to take responsibility for any problems that arise as a result of the consultation.

We should be well aware that people with excellent specialized skills are novices in fields other than their own. Even in major media outlets, there are cases where people with specialized skills comment on issues outside their field of expertise. This is very disappointing, and comments on issues outside of one's expertise are often misguided. The correct professional response would be to refuse to comment on issues outside of one's expertise. It also goes without saying that we should not ask people with great expertise to do work that is outside their expertise. Thus, it is not appropriate to name untrained maintainers as a consultation contact, but rather, it should be clearly stated that maintainers are not a consultation contact.

Maintainers have no incentive to take their time to resolve disputes between individuals. The existing codes make the maintainers bear the cost of ensuring the diversity of the community. It is hard to imagine that forcing the maintainer to deal with the difficult problem of resolving disputes between individuals without paying any compensation would work. If a project member believes that he or she has been victimized, he or she should not expect the project's consultation service to function properly, but should seek an official contact outside the project. Also, if a project truly values the diversity of its members, it would be more constructive to promote the establishment of a consultation service for OSS projects by an organization that can be trusted to some extent. There is no guarantee that fair decisions will be made in such services, but if trained experts are consulted, better results can be expected than relying on novice maintainers. It is also expected that the criteria for judgment will become relatively uniform. To hire such an expert, however, funds need to be raised.


### Criteria for identifying violations are not clearly stated

For consulters, it is important to note that the maintainers should not be trusted unconditionally and there is no guarantee that the maintainers will side with the consulter. If some rules contain penal provisions with ambiguous criteria for violation, such provisions can
be arbitrarily administered by decision makers simply to impose private penalties on members they don't like. And that is often a reality. To avoid arbitrary enforcement of rules, the criteria for violation need to be objective.

Maintainers may want to make the rules that allow the maintainers to make arbitrary decisions to allow for flexible operations in unpredictable situations. Unfortunately, such rules and their operation are in fact quite common outside of the Internet. However, if the maintainers have no intention to make an objective decision from the beginning, then everything will ultimately be determined by the likes and dislikes of the maintainers. Members other than the maintainers have no choice but to trust that the maintainers will make a fair decision, and there is no difference between having rules and not having rules.


### The only thing maintainers can do is to ban violators, which is not much of a deterrent to violations

If the violator participates in a project using pseudonyms, it is easy for the violator to return to the project pretending to be a new participant after being banned from the project. This has happened countless times in the past. The "consequences" of banning violators sounds just ridiculous. Nowadays, it is not uncommon to be banned from social networking sites for incomprehensible reasons. Since being banned is the most you can get, such "consequences" are equivalent to nothing.


Frankly, I cannot help but be surprised that so many prominent OSS projects have already adopted such codes of conduct that are ambiguous and of questionable effectiveness.

A quick way to improve community diversity would be to ensure transparency in all important deliberative processes. However, such an operation will undoubtedly lead to an increased workload on the maintainers. I believe that we should start by improving the treatment of maintainers.


## The reason to create a new code of conduct

If a code of conduct is to be considered a binding contract, it will be necessary to clarify how it is positioned in relation to the software distribution license. It would also require a reason to add a further agreement in addition to the distribution license. It may be possible to incorporate the code of conduct into the software distribution license.

On the other hand, it is also possible to make the code of conduct a non-binding goal of effort, and only aim to get the members to agree with the philosophy. In this case, the code of conduct could include the kinds of things that are usually not included in software distribution licenses, and thus issues that could not be solved by a software distribution license alone can be addressed.


The specific problem I am having with my project is what is called the burnout of OSS developers [4, 5, 6, 7], and this is not what is written in the existing codes of conduct, etc. In OSS projects, software needs to be maintained continuously, and this requires a continuous effort to be devoted to the maintenance. This becomes especially evident when the software being developed in a project becomes large in scale. However, OSS developers have little or no financial incentive to continue maintenance and development. Many users of OSS expect the projects to be maintained for a long period of time, even though they do not pay a fee. The result is that many OSS developers stop maintaining projects and developing new features much sooner than users expect. This may not be a very new problem either, but there is no established way to solve it.

The Community Guidelines for Sustainability of Open-Source Ecosystem aim to solve the OSS developers' burnout problem. It sets the goal of the project members' efforts to promote the awareness that if a company makes a profit from the commercial use of OSS, they should contribute to relevant projects. The adoption of the guidelines by a large number of OSS projects will make the general public at least aware of the burnout problem of OSS developers.


## To realize actual profit distribution

One reason why companies have not provided substantial financial support for OSS projects in the past may be because there was no infrastructure for this purpose. If a company actually wants to provide financial support to an OSS project, the simplest way is that the company provides support to each individual contributor. However, this requires that the company knows the status of the project in detail. Especially if the project is dependent on other projects, a very large number of contributors can be candidates for support. It may be too complicated for each company to evaluate a large number of contributors and determine the amount of support for each.

If companies provide bulk support to each project or a set of related projects, it will be necessary to establish criteria for fair and objective distribution of funds among and within projects. This requires an objective and fair method of evaluating each member's contribution to the project. For example, if the contribution of each member is simply evaluated by the number of lines of source code rewritten, this is hardly fair and will lead to rampant and meaningless rewriting of source code, resulting in many complaints from project contributors. Objective evaluation of contributions is not simple and requires academic research. At first glance, the construction of such an evaluation method seems not easy.

I expect that as firms offering the above services emerge and compete with each other, capitalist mechanisms will optimize the criteria for the distribution of funds. In this scenario, several firms offering the above services will first emerge. Each of these firms will implement different distribution criteria for funds and publish those criteria. The firms will then start services to distribute the funds according to their criteria after charging a fee. Each OSS project designates the firm it considers to have the best criteria when it receives the funds. Firms that implement better criteria and services will earn more fee income as they are used more often. In this way, the criteria for distribution of funds are optimized by capitalism. Also, public disclosure of the amount of support for projects by each company using OSS would give a promotional meaning to the company's support for OSS projects. This would be expected to stimulate more support for OSS projects.

In any case, the first step is to make it commonplace that companies that use OSS provide financial support to OSS projects. Then, firms that provide the above services would start to emerge.


## Regarding accounting for the payments

If a company provides financial support for a project as a donation, various restrictions may arise in some countries.

Here we consider the case where a company does not make a donation to a project, but instead enters into an agreement to contract out the development to an individual developer. Under this arrangement, the company would spend the funds under a category such as "research and development expenses." However, the contract would have to be for some large, collective modification to the software. In addition, since it is not known whether the development will succeed or not in advance, it becomes troublesome to make agreements related to the development process, such as the establishment of the purpose of development.

One way to avoid this complication is to have the company pay for the management and operation of the CI system operated by the project. In this method, the maintainers and developers involved in the project jointly manage and operate the CI system, and the project requires the use of this CI system when committing the code as a project policy. In this way, the fee for the use of this CI system can be set up as financial support for the project from the company. This usage price can be set freely according to the situation, independent of the frequency of use of the CI system.

One of the advantages of adopting the method in which companies pay for the management and operation of CI systems is that it is clear from the beginning that the purpose of paying fees is for the management and operation of CI systems, and there are no complications in making agreements regarding the implementation of the contract. Since there is relatively little need to add value to the CI system by newly modifying its functionality, and the benefits to be gained by entering into a contract are clear from the start, the contract can be simple and straightforward. In addition, unlike methods such as selling advertising space on a project's website, it is possible to set the price as a discretionary price, and this has the advantage of allowing the price to be set freely.

In general, companies tend to avoid signing contracts directly with individuals. Therefore, it may be easier for companies to pay usage fees for CI systems to some legal entity, and then that entity pays the fees to the maintainer and developer. In this scheme, the maintainer and developer sign an agreement for the management of the CI system with this entity and receive a fee from this entity. Alternatively, the maintainer and developer may become employees of the entity and receive fees in the form of salaries. This legal entity may be a corporation established by the maintainer and developer. Services provided by an outside vendor may also be used for the payments in this scheme. Depending on the form of the contract, default may occur if the management and operation of the CI system is not successful. Default will almost never occur if the payment for the management and operation of the CI system is made in the form of deferred payment after the contract period is over, and the contract is renewed every month. In addition, various tax-saving measures can be taken with this scheme, but these are not discussed here because circumstances differ from country to country.


## Acknowledgement

I thank Mr. Eiji Ito for his expertise and assistance in writing this document.


## References

[1] Tourani, Parastou, Bram Adams, and Alexander Serebrenik. "Code of conduct in open source projects." 2017 IEEE 24th international conference on software analysis, evolution and reengineering (SANER). IEEE, 2017.

[2] [https://en.wikipedia.org/wiki/Code of conduct](<https://en.wikipedia.org/wiki/Code of conduct>)

[3] https://github.com/domgetter/NCoC

[4] https://www.businessinsider.com/open-source-developers-burnout-low-pay-internet-2022-3

[5] https://trstringer.com/oss-compensation-broken/

[6] https://www.vice.com/en/article/43zak3/the-internet-was-built-on-the-free-labor-of-open-source-developers-is-that-sustainable

[7] https://staltz.com/software-below-the-poverty-line.html


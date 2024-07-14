
# The Community Guidelines to Ensure Fair Rewards for OSS Projects

Version 0.7, 2024-07-07

Copyright Naoki Shibata 2024.

This document is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).


## What is it?

These are non-binding community guidelines intended to be used as a
code of conduct for OSS projects. The guidelines have the following
features.

* The guidelines aim to alleviate burnout problems for OSS developers.
* The guidelines include portions of the existing codes of conduct, but
  written to be as objective as possible concerning the criteria for
  identifying violations.
* Clearly states the positioning, that it is non-binding, and that it
  does not stipulate penalties for violations.
* The guidelines are designed to avoid adding new responsibilities to
  the project maintainer.


## How can I use it in my project?

Please copy
[CODE_OF_CONDUCT.md](https://github.com/shibatch/nofreelunch?tab=coc-ov-file)
into the root directory of your project.  It is distributed under
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).


## Introduction

As the number of individuals from diverse backgrounds participating in
open-source and free software projects continues to grow, an
increasing number of such projects are adopting a code of conduct with
the objective of ensuring that all participants have equal opportunity
to contribute to the project.

A code of conduct is a set of rules that defines the normative
behavior and responsibilities of individuals, parties, and
groups. Typically, they are created for employees of a company in
order to protect the company and to inform employees of the company's
expectations. In general, codes of conduct in OSS projects state
the following items [1][2].

* Respect and welcome diversity.
* Be patient, kind, do the best for the community, be considerate and
  cooperative.
* Condemn sexist/racist language, insults, jokes, violence or threats
  that harass marginalized people.
* Report unacceptable behavior to a specific group of team members who
  usually have the authority to determine appropriate action.


## Problems with existing codes of conduct

However, the issues addressed by these codes of conduct are not
novel. Rather, they are long-standing concerns that have been present
for some time, and these issues have been acknowledged and addressed
to some extent. The recent emergence of these codes is
perplexing. What prompted the introduction of these codes, and what
are the benefits of having a code of conduct? What would be the
consequences of not having one? There are numerous questions that
remain unanswered.

In fact, there are OSS projects that oppose the introduction of such a
code of conduct, and some strong opponents explicitly choose "No Code
of Conduct" for their projects [1][3].

I also have the following concerns in introducing a code of conduct to
my project.

* Criteria for identifying violations are not clearly stated.
* The purpose of presenting such a code is not clearly stated.
* The consequences for violations are not clearly stated. In practice,
  all the maintainer can do is to ban the user at best.
* It has a patternalistic nature, and the idea of secretly telling the
  maintainer about the victimization and asking the maintainer to
  resolve it seems terribly childish.
  * Maintainers are not the parents of the project members.
  * Most OSS project maintainers are not experts in resolving disputes
    between individuals.
  * There is no guarantee that the maintainers will side with the
    victimized party.
* These codes make the maintainers bear the cost of ensuring the
  diversity of the community.
  * If the person alleging victimization secretly consults with the
    maintainer, it is often not easy for the maintainer to respond to
    that consultation.
    * If the claim of victimization is not valid, the maintainer needs
      to convince the person of this.
    * If the maintainer inadvertently chooses wrong words, or even if
      everything is handled properly, the maintainer could also be
      accused of being a perpetrator.
    * In some cases, such as when the person suffers from mental
      illness, professional expertise is required in order to provide
      appropriate consultation. It is not easy for an untrained
      maintainer to notice mental illness, but the maintainer may
      still need to take responsibility for any problems that arise as
      a result of the consultation.
  * Maintainers have no incentive to take the time to resolve disputes
    between individuals.

Even if the code of conduct can restrict some actions of members, it
is only on the web pages related to the project. The mere maintainers
of an OSS project do not have the authority to tell project
participants what to or not to say on social networking sites
unrelated to the project. It is a difficult task to just simply make
factual determinations in cases of suspected illegal activity, and OSS
project maintainers are typically not trained to do such things.

The project should not impose private penalties for offensive comments
made by members on social networking sites that are not related to the
project. Even if a member's non-project-related behavior has been
found by an official agency to be illegal, whether the project should
take any action in response is a matter for careful deliberation. It
is the role of the authorities to punish members for illegal behavior,
not the project maintainers, unless the authorities ask the
maintainers to do something specific. The only thing that members of
the project, including the maintainers, should do is to preserve
evidence and to report any ongoing illegal activity related to the
project to the public authorities.

If some rules contain penal provisions with ambiguous criteria for
violation, such provisions can be arbitrarily administered by decision
makers simply to impose private penalties on members they don't
like. And that is often a reality. To avoid arbitrary enforcement of
rules, the criteria for violation need to be objective.

From the standpoint of guaranteeing freedom of speech, it is rather
better not to have rules or anything like that restricting speech in
non-project related venues. Maintainers are not there to punish
members. Banning a member in a project should be done out of necessity
in order to defend the project, not to punish the member. If a project
member believes that he or she has been victimized, he or she should
not expect the project's consultation service to function properly,
but should seek an official contact outside the project. Also, if a
project truly values the diversity of its members, it would be more
constructive to promote the establishment of a consultation service
for OSS projects by an organization that can be trusted to some
extent. There is no guarantee that fair decisions will be made in such
services, but if trained experts are consulted, better results can be
expected than relying on novice maintainers. And to hire such experts,
funds need to be raised.

Even in major media outlets, there are cases where people with
specialized skills comment on issues outside their field of
expertise. However, we should be well aware that people with excellent
specialized skills are novices in fields other than their
own. Furthermore, we should not ask people with excellent specialized
skills to do work outside of their field of expertise. It is not
appropriate to name untrained and unpaid maintainers as a consultation
contact, but rather, it should be clearly stated that maintainers are
not a consultation contact.

Frankly, I cannot help but be surprised that so many prominent OSS
projects have already adopted such codes of conduct that are ambiguous
and of questionable effectiveness.


## The reason to create a new code of conduct

If a code of conduct is to be considered a binding contract, it will
be necessary to clarify how it is positioned in relation to the
software distribution license. It would also require a reason to add a
further agreement in addition to the distribution license. It may be
possible to incorporate the code of conduct into the software
distribution license.

On the other hand, it is also possible to make the code of conduct a
non-binding goal of effort, and only aim to get the members to agree
with the philosophy. In this case, the code of conduct could include
the kinds of things that are usually not included in software
distribution licenses, and thus issues that could not be solved by a
software distribution license alone can be addressed.


The specific problem I am having with my project is what is called the
burnout of OSS developers [4, 5, 6, 7], and this is not what is written in
the existing codes of conduct, etc. In OSS projects, software needs to
be maintained continuously, and this requires a continuous effort to
be devoted to the maintenance. This becomes especially evident when
the software being developed in a project becomes large in scale.
However, OSS developers have little or no financial incentive to
continue maintenance and development. Many users of OSS expect the
projects to be maintained for a long period of time, even though they
do not pay a fee. The result is that many OSS developers stop
maintaining projects and developing new features much sooner than
users expect. This may not be a very new problem either, but there is
no established way to solve it.

The Community Guidelines to Ensure Fair Rewards for OSS Projects aim
to solve the OSS developers' burnout problem. It sets the goal of the
project members' efforts to promote the awareness that if a company
makes a profit from the commercial use of OSS, a portion of the profit
should be returned to the project. OSS is software that can be used
free of charge, but obviously it does not prohibit the return of
profits made through the use of OSS. If it becomes widely recognized
that companies are natural to return a portion of the profits earned
from the use of OSS to the projects, and if companies' codes of
conduct incorporates financial support for OSS projects, we can expect
to see significant progress toward solving the burnout problem. The
adoption of the guidelines by a large number of OSS projects will make
those companies at least aware of the burnout problem of OSS
developers.


## To realize actual profit distribution

One reason why companies have not provided substantial financial
support for OSS projects in the past may be because there was no
infrastructure for this purpose. If a company actually wants to
provide financial support to an OSS project, the simplest way is that
the company provides support to each individual contributor. However,
this requires that the company knows the status of the project in
detail. Especially if the project is dependent on other projects, a
very large number of contributors can be candidates for support. It
may be too complicated for each company to evaluate a large number of
contributors and determine the amount of support for each.

If companies provide bulk support to each project or a set of related
projects, it will be necessary to establish criteria for fair and
objective distribution of funds among and within projects. This
requires an objective and fair method of evaluating each member's
contribution to the project. For example, if the contribution of each
member is simply evaluated by the number of lines of source code
rewritten, this is hardly fair and will lead to rampant and
meaningless rewriting of source code, resulting in many complaints
from project contributors. Objective evaluation of contributions is
not simple and requires academic research. At first glance, the
construction of such an evaluation method seems not easy.

I expect that as firms offering the above services emerge and compete
with each other, capitalist mechanisms will optimize the criteria for
the distribution of funds. In this scenario, several firms offering
the above services will first emerge. Each of these firms will
implement different distribution criteria for funds and publish those
criteria. The firms will then start services to distribute the funds
according to their criteria after charging a fee. Each OSS project
designates the firm it considers to have the best criteria when it
receives the funds. Firms that implement better criteria and services
will earn more fee income as they are used more often. In this way,
the criteria for distribution of funds are optimized by capitalism.
Also, public disclosure of the amount of support for projects by each
company using OSS would give a promotional meaning to the company's
support for OSS projects. This would be expected to stimulate more
support for OSS projects.

In any case, the first step is to make it commonplace that companies
that use OSS provide financial support to OSS projects. Then, firms
that provide the above services would start to emerge.


## Conclusion

The Community Guidelines to Ensure Fair Rewards for OSS Projects are
community guidelines aiming to solve the burnout problem of OSS
developers.

* The guidelines are not legally binding, but are positioned as a soft
  rule that would be a bit uncool if violated.
* The guidelines solve the burnout problem through the PR effect on
  the companies. In other words, if a company that makes commercial
  use of OSS or free software refuses to adopt these guidelines, it
  would appear to be a declaration of their desire to continue
  free-riding.
* Adopting these guidelines will make it clear that the project is
  requesting financial support.
* By adopting the guidelines, the project can facilitate the creation
  of an infrastructure for the distribution of funds.


## References

[1] Tourani, Parastou, Bram Adams, and Alexander Serebrenik. "Code of
conduct in open source projects." 2017 IEEE 24th international
conference on software analysis, evolution and reengineering
(SANER). IEEE, 2017.

[2] [https://en.wikipedia.org/wiki/Code of conduct](<https://en.wikipedia.org/wiki/Code of conduct>)

[3] https://github.com/domgetter/NCoC

[4] https://www.businessinsider.com/open-source-developers-burnout-low-pay-internet-2022-3

[5] https://trstringer.com/oss-compensation-broken/

[6] https://www.vice.com/en/article/43zak3/the-internet-was-built-on-the-free-labor-of-open-source-developers-is-that-sustainable

[7] https://staltz.com/software-below-the-poverty-line.html

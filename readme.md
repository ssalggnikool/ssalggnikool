# My projects no longer live on GitHub

Over the last couple of years, GitHub has been turned into a distribution channel for Microsoft's LLMs,
transforming a collaborative workspace into a machine that extracts surplus value from free software maintainers.

I am personally no longer willing to host any of my projects here. All my repositories are slowly
being either archived or deleted. If you're looking for them, feel free to check them out on [Codeberg].

###### original text written by [lívia](https://codeberg.org/livia)

## LLM-driven features you can't turn off

The tech monopoly harvests open-source repositories as raw material to train its proprietary LLMs,
commodifying uncompensated digital labour[^24].

GitHub lets anyone open issues and pull requests using Copilot[^1]. Projects can't opt out of
receiving them, and nothing indicates that Copilot wrote them[^2]. By September 2025, the
most-upvoted discussion of the year on GitHub's own community forum was a request to block this,
and the second was a request to be able to turn off Copilot code review[^9]. Neither was resolved.
Around the same time, GitHub's CEO told developers to embrace AI or get out[^10], then stepped
down, and GitHub was folded into Microsoft's CoreAI group[^5].

In March 2026, Copilot was found editing pull request descriptions written by other people to
insert promotional "tips", including one for a third-party app, in more than 11,000 pull
requests[^6]. GitHub called it a "programming logic issue" and removed it within a day[^16]. But it
also confirmed Copilot had been adding these tips to its own pull requests for some time, and
nobody had been told that Copilot had permission to rewrite text other users wrote.

## Your code is the training data

Microsoft's head of AI has described content on the open web as effectively "freeware" for
training[^4], disregarding copyright and software licensing.

The legal route for enforcing attribution has also narrowed. In September 2026 the Ninth Circuit
upheld the dismissal of the DMCA claims in *Doe v. GitHub*, reasoning that Copilot generates new
code that never contained the original license notices, so nothing was "removed"[^17][^18]. The
court didn't rule on ordinary copyright infringement, but the DMCA argument, the one that made
attribution-stripping expensive, is now closed in that circuit.

## Reliability and pricing

curl ended its bug bounty on January 31, 2026, after being flooded with fabricated, largely
AI-generated vulnerability reports[^3][^11]. tldraw started auto-closing all external pull
requests[^12]. By GitHub's own numbers, merged pull requests went from 25 million a month in
January 2023 to 90 million a month by March 2026[^13], and every rejected one also had to be read
by someone.

GitHub's response has been to let maintainers disable pull requests entirely, restrict them to
collaborators, or cap how many outsiders can open[^14][^15][^13].

GitHub has been migrating to Azure while traffic from coding agents grows faster than it planned
for. One third-party tracker counted 48 major outages between May 2025 and April 2026[^19]. In
April 2026 Mitchell Hashimoto announced Ghostty is leaving GitHub because outages were blocking his
work almost daily[^20]. Zig moved to Codeberg in November 2025, citing unreliable and neglected
GitHub Actions and GitHub's AI push, which conflicts with Zig's own ban on LLM-written
contributions[^21][^22].

In December 2025, GitHub also announced a per-minute fee for self-hosted Actions runners, meaning a
charge for running CI on your own hardware. It postponed the fee after the backlash[^23], but
didn't cancel it.

[Codeberg]: https://codeberg.org/paige

[^1]: https://github.com/orgs/community/discussions/159749
[^2]: https://github.com/orgs/community/discussions/159749#discussioncomment-13205901
[^3]: https://arstechnica.com/gadgets/2025/05/open-source-project-curl-is-sick-of-users-submitting-ai-slop-vulnerabilities/
[^4]: https://www.theregister.com/2024/06/28/microsoft_ceo_ai/
[^5]: https://arstechnica.com/gadgets/2025/08/github-will-be-folded-into-microsoft-proper-as-ceo-steps-down/
[^6]: https://www.theregister.com/2026/03/30/github_copilot_ads_pull_requests
[^7]: https://github.blog/news-insights/company-news/updates-to-github-copilot-interaction-data-usage-policy/
[^8]: https://www.heise.de/en/news/Only-with-opt-out-GitHub-will-train-Copilot-models-with-user-data-in-the-future-11226787.html
[^9]: https://www.theregister.com/2025/09/05/github_copilot_complaints/
[^10]: https://www.businessinsider.com/github-ceo-developers-embrace-ai-or-get-out-2025-8
[^11]: https://daniel.haxx.se/blog/2026/01/26/the-end-of-the-curl-bug-bounty/
[^12]: https://tldraw.dev/blog/stay-away-from-my-trash
[^13]: https://www.coderabbit.ai/blog/github-gives-maintainers-a-throttle-for-the-ai-pull-request
[^14]: https://www.theregister.com/2026/02/03/github_kill_switch_pull_requests_ai/
[^15]: https://github.blog/open-source/maintainers/welcome-to-the-eternal-september-of-open-source-heres-what-we-plan-to-do-for-maintainers/
[^16]: https://www.neowin.net/amp/github-copilot-ads-in-pr-were-due-to-a-programming-logic-issue-claims-microsoft/
[^17]: https://cdn.ca9.uscourts.gov/datastore/opinions/2026/09/16/24-7700.pdf
[^18]: https://thenextweb.com/news/ninth-circuit-github-copilot-dmca-copyright-ruling
[^19]: https://blog.incidenthub.cloud/github-reliability-outage-history-2025-2026
[^20]: https://mitchellh.com/writing/ghostty-leaving-github
[^21]: https://ziglang.org/news/migrating-from-github-to-codeberg/
[^22]: https://devclass.com/2025/11/27/zig-project-ditches-github-for-codeberg-but-move-could-be-costly/
[^23]: https://www.techzine.eu/news/devops/137396/github-bends-to-criticism-and-delays-paid-self-hosting-of-runners/
[^24]: https://link.springer.com/article/10.1007/s00146-023-01692-3

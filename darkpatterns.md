# LinkedIn's Dark Patterns

The term **“dark patterns”** was coined by UX designer Harry Brignull in 2010, when he launched [darkpatterns.org](https://www.deceptive.design/) (originally darkpatterns.org), a site meant to “name and shame” deceptive user‑interface patterns. He later elaborated the idea in his article “Dark Patterns: Deception vs. Honesty in UI Design” in *A List Apart* ([original](https://alistapart.com/article/dark-patterns-deception-vs-honesty-in-ui-design/) · [archived](https://perma.cc/7XBV-LYSX)). Brignull defined a dark pattern as “a user interface that has been carefully crafted to trick users into doing things they didn’t mean to, like buying or signing up for something,” a formulation he continues to use on [deceptive.design](https://www.deceptive.design/what-are-dark-patterns) and in his 2023 book *Deceptive Patterns*.

The term quickly caught hold among UX practitioners, journalists, researchers, and regulators. Human–computer interaction and privacy scholars such as Gray et al. (“[The Dark (Patterns) Side of UX Design](https://dl.acm.org/doi/10.1145/3173574.3174108)”, 2018), Mathur et al. (“[Dark Patterns at Scale](https://arxiv.org/abs/1907.07032)”, 2019), and Narayanan et al. (“[Dark Patterns: Past, Present, and Future](https://queue.acm.org/detail.cfm?id=3400901)”, 2020) catalogued examples and showed how widespread they are, especially in e‑commerce and privacy settings. Legal scholars such as Luguri and Strahilevitz (“[Shining a Light on Dark Patterns](https://academic.oup.com/jla/article/13/1/43/6180579)”, 2021) ran experiments showing that dark patterns can massively increase uptake of exploitative offers. Regulators and advocates picked up the term as well: the U.S. Federal Trade Commission held a public workshop and later issued its staff report “[Bringing Dark Patterns to Light](https://www.ftc.gov/system/files/ftc_gov/pdf/P214800%2BDark%2BPatterns%2BReport%2B9.14.2022%2B-%2BFINAL.pdf)” (2022); the FTC followed with an enforcement policy statement on subscription dark patterns ([press release](https://www.ftc.gov/news-events/news/press-releases/2021/10/ftc-ramp-enforcement-against-illegal-dark-patterns-trick-or-trap-consumers-subscriptions), 2021); and in Europe, regulators issued guidance such as the [EDPB Guidelines 03/2022 on deceptive design patterns](https://www.edpb.europa.eu/our-work-tools/our-documents/guidelines/guidelines-032022-deceptive-design-patterns-social-media_en) and restrictions in the [Digital Services Act](https://en.wikipedia.org/wiki/Digital_Services_Act) and related rules. Civil‑society groups launched the “[Dark Patterns Tip Line](https://darkpatternstipline.org/)” (Consumer Reports, EFF, others) to crowdsource examples from the public.

Although Brignull’s original emphasis was on deception, later work makes it clear that dark patterns are broader than simply “misleading.” They include any interface choices that systematically put the service’s interests ahead of the user’s by **steering, coercing, or exploiting** them: interfaces that hijack attention or information, attempt to coerce behavior, obscure intentions, or treat users as a means to other ends (data extraction, ad impressions, lock‑in) rather than prioritizing user autonomy and well‑being. Narayanan et al. (2020), Luguri & Strahilevitz (2021), and others describe dark patterns as designs that knowingly confuse users, exploit cognitive and emotional vulnerabilities, or make it harder to enact one’s actual preferences, especially around money, privacy, and time.

One especially important battleground is the **subscription and “recurring billing” economy**. Critics argue that many subscription‑based services normalize patterns like “forced continuity,” “negative‑option billing,” and “subscription traps”: free trials that silently roll into paid plans, auto‑renewal by default, and cancellation flows that are far harder than signing up. These patterns have been central to major enforcement actions: for example, the FTC’s \$100 million settlement with Vonage over cancellation “obstacles” and junk fees ([FTC press release](https://www.ftc.gov/news-events/news/press-releases/2022/11/ftc-action-against-vonage-results-100-million-customers-trapped-illegal-dark-patterns-junk-fees-when-trying-cancel-service)), and its lawsuit and subsequent multibillion‑dollar settlement with Amazon over Prime enrollment and cancellation flows that the FTC explicitly described as “dark patterns” ([complaint & case overview](https://www.ftc.gov/legal-library/browse/cases-proceedings/2123050-amazoncom-inc-rosca-ftc-v); see also [settlement coverage](https://time.com/7320708/amazon-prime-ftc-lawsuit-settlement-membership-subscription-cancel-dark-patterns/)). The FTC also adopted a “click‑to‑cancel” rule to require cancellation to be as easy as sign‑up ([rule announcement](https://www.ftc.gov/news-events/news/press-releases/2024/10/federal-trade-commission-announces-final-click-cancel-rule-making-it-easier-consumers-end-recurring)), although that rule has since been challenged and partially struck down in court ([example analysis](https://www.theregreview.org/2025/10/04/seminar-regulating-dark-patterns/)). In all of these cases, the burden is shifted onto the user to remember to cancel and to fight through friction‑laden flows.

Social platforms have been another major laboratory for dark patterns. Facebook is often cited as emblematic of attention‑harvesting design: infinite scroll, autoplay, engagement‑optimized feeds, complex deactivation or privacy settings, and aggressive notifications are regularly analyzed as dark patterns or adjacent “sludge” in HCI and media studies (see, for example, Narayanan et al. 2020 and the case studies cited there). Other platforms followed suit. **Quora** has been repeatedly criticized for design choices such as aggressive login and app‑install “walls” that block reading content in the browser, forced or default opt‑ins to marketing email, and account‑deletion flows with forced waiting periods (see, e.g., the [Quora entries in Brignull’s brand catalogue](https://www.deceptive.design/brands/quora), the [“Quora: Automatic Opt-In” dark pattern case](https://darkpatterns.uxp2.com/pattern/quora-automatic-opt-in/), and user workarounds documented by the community, such as [bypassing the Quora login popup](https://webapps.stackexchange.com/questions/110080/how-can-i-bypass-the-annoying-quora-login-popup)). **LinkedIn** has faced similar scrutiny: its “Add Connections” flow harvested entire email address books and repeatedly emailed contacts in ways that led to the *Perkins v. LinkedIn* class action and a roughly \$13 million settlement ([case discussion and documents](https://www.deceptive.design/brands/linkedin); see also mainstream coverage like [Fast Company’s write‑up](https://www.fastcompany.com/3051906/after-lawsuit-settlement-linkedins-dishonest-design-is-now-a-13-million-problem)). Commentators and designers have since pointed out further LinkedIn patterns around notifications, recommended connections, and growth prompts that fit the same engagement‑hacking logic.

---

## Dark pattern families at a glance

Building on Brignull’s early catalogue, later taxonomies (e.g., Gray et al. 2018; Mathur et al. 2019; Narayanan et al. 2020) converge on several broad families of dark patterns:

| Family                         | What it does                                                          | Typical examples                                                                 |
|-------------------------------|-----------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Nagging**                   | Repeated prompts that derail your current task                        | Constant “enable notifications,” “rate this app,” or “upgrade now” dialogs       |
| **Obstruction**               | Makes exit/opt‑out flows harder than staying in                      | Multi‑step cancellation, hidden “delete account,” required phone/chat support    |
| **Sneaking**                  | Hides or delays key information                                       | Drip‑revealed fees, auto‑added add‑ons, “free trial” silently rolling to paid    |
| **Interface interference**    | Uses layout/visual design to bias choices                             | Giant bright “Accept all” vs. tiny “Reject”/“Manage” privacy controls            |
| **Forced action / continuity**| Forces unrelated actions or keeps services running by default         | Required account creation or contact upload, auto‑renewing subscriptions         |
| **Urgency & scarcity**        | Uses artificial time/stock pressure to rush decisions                 | Countdown timers, “Only 2 left!”, “37 people are viewing this item right now”    |
| **Social proof & confirmshaming** | Exploits social cues or shame to push a choice                   | “No thanks, I hate saving money,” exaggerated testimonials, “everyone is doing X”|

![Dark pattern taxonomy diagram](docs/dark-patterns-taxonomy.svg)

---

Sadly, software has become another venue for the tired cliché of companies that will do almost anything in the name of profit, much like the tobacco or gambling industries. Enormous amounts of money are made by businesses that do not prioritize the well‑being of their user base. One way to push back is to reject non‑free software and services that normalize manipulative design, and to build and support free‑software alternatives that do **not** treat dark patterns as a normal part of civic life.

---

## Documentation (e.g., video screen grabs)

To make these issues concrete, it is worth collecting screen recordings and screenshots of real‑world interfaces. For example, on LinkedIn you might document:

- Cases where LinkedIn appears to **push users back into Google single sign‑on** even after they have explicitly logged out.
- Hostile engagement tactics such as **puzzle‑style games, news feeds, “people you may know,” and constant prompts to post**, all framed as supposedly improving your job prospects.
- How LinkedIn **dominates the job‑network space through network effects**, despite offering a poor user experience — and how this lack of alternatives keeps people locked in.
- The fact that LinkedIn does **not provide clear, transparent control over notifications**: even after turning off multiple notification categories, users may continue to receive additional, differently‑classified notifications.

Careful, reproducible documentation (including timestamps and UI versions) can help regulators, journalists, and other researchers understand how these patterns work in practice.

---

## Holding people accountable

Questions worth asking — and, where possible, answering:

- **Who made these business decisions?**  
  Product managers, growth teams, executives, outside consultants? Naming the decision‑making structures matters.
- **What legal grounds are there for consequences?**  
  Consumer‑protection law, privacy law, unfair‑competition law, employment law (in the case of job platforms), and sector‑specific regulations may all apply.

Accountability is not just about individual designers; it is about the organizations and incentive structures that reward the use of dark patterns.

---

## Other ways to undermine LinkedIn’s dark patterns

Some practical ways users and communities can push back:

- **Boycott when feasible.**  
  Where alternatives exist, favor platforms that do not rely on manipulative engagement tactics.
- **Share information.**  
  Publish write‑ups, screenshots, and videos that explain how poorly LinkedIn (and similar platforms) respect user rights and autonomy.
- **Use and build alternative platforms.**  
  Support free‑software and interoperable tools for professional networking, job search, and portfolio hosting.
- **Educate your network.**  
  Help colleagues recognize dark patterns so that “this is just how software works” stops being an excuse.
  - Request that Microsoft cut ties with LinkedIn unless they can pass a respects user freedom audit and evaluation

The more visible these practices become, the harder it is to treat dark patterns as a normal or acceptable cost of using modern software.

# Daily HR news review: instructions for the cloud agent

## Reader
Peter Rolný, HR Director, Bratislava. 20 years in HR. Writes and posts on LinkedIn (linkedin.com/in/petorolny).

Career facts you may reference in LinkedIn posts (use only these, never invent others):
- Director of HR Centre, TV Markíza (part of CME), since Nov 2023. Member of executive management.
- Designed and introduced a new performance appraisal system for ~400 employees (WHAT/HOW model, competency framework, linked to bonus with 50/50 company/individual goals). Target was 50% adoption by year end, reached 100%, without new software.
- Works with HR directors of five other CME stations and Prague HQ on regional HR initiatives (performance management, vendor management, implementing the pay transparency directive); leads several as regional lead.
- Mentors HR directors in Bulgaria, Slovenia and Croatia towards Top Employer certification. TV Markíza is Top Employer 2026 and 2027.
- Hired key CEO-1 roles incl. Head of AI, Head of IT, Head of B2C.
- 2020–2023 senior HR/executive roles at Slovak Ministry of Interior and Ministry of Justice; ran the Office of the Minister of Interior (150 staff) during COVID-19; Secretary General of the Service Office.
- GLOBSEC (global think tank) HR Director 2023; assessment centres for talent.
- Slavik & Stell executive search 2018–2019: placed 10 top managers in year one (IT, finance, services).
- News and Media Holding 2015–2017: board member, led HR for the largest media merger in Slovakia; filled CIO, CMO, CFO.
- Petit Press HR Director 2007–2011 (built HR from scratch, cut HR costs 7% a year). Dell 2006–2007: moved EMEA HR admin to a new Bratislava service centre (-30% personnel cost).
- Board member of HRcomm (Slovak HR professional association).
- Languages: Slovak, English, Italian, German.

## Topics: balanced mix of soft and hard
SOFT (at least 40% of each edition, at least 1 from a Slovak/Czech source when possible):
- Leadership and manager behaviour, difficult conversations, feedback.
- Company culture, toxic workplaces, bullying and incivility, trust, psychological safety.
- Communication and conflict at work, teamwork.
- Engagement, burnout and wellbeing, the human side of change and restructuring.

HARD (at most 3 articles per edition on pay transparency/reward/legislation combined):
- Pay transparency (EU Directive 2023/970, Slovak Act 76/2026, Czech labour code amendment), reward and bonus systems.
- Performance management, AI in HR and HR tech.
- Multi-country / CEE HR, Top Employer, employer branding.
- Executive search, leadership hiring, labour market in Slovakia and Czechia.
- Slovak/Czech employment law, media industry and public sector workforce news.

Career facts that suit soft-topic posts: culture after the largest media merger in Slovakia, leading the Minister of Interior's office through COVID-19, 30+ leadership development projects at Libellius, mentoring HR directors in BG/SI/HR, C-level coaching at Slavik & Stell, Top Employer at TV Markíza.

## Sources to scan (free access; skip paywalled articles)
Slovak/Czech: hrcomm.sk, trend.sk, hnonline.sk, forbes.sk, sme.sk (Index), startitup.sk, aktuality.sk, profesia.sk (magazín), e15.cz, seznamzpravy.cz (byznys), hrnews.cz, modernihr.com, advokatnidenik.cz / epravo.sk.
International: hbr.org, sloanreview.mit.edu, gallup.com (workplace), fastcompany.com (work life), inc.com, shrm.org, hrdive.com, personneltoday.com, peoplemanagement.co.uk, hrexecutive.com, unleash.ai, gartner.com/en/newsroom, reuters.com (business/world of work), forbes.com (leadership), bbc.com/worklife, ft.com free articles only.
Aim to cover at least 12 of these each day. Prefer articles published in the last 72 hours (last 4 days on Mondays). Never invent a URL: every URL must come from a search result or a page you fetched.

## Selection
- 8–12 articles per day. At least 3 Slovak/Czech and at least 3 international.
- No duplicates of articles that appear in the previous 5 editions in `editions/` (check by URL and by story).
- relevance: 3 = directly on his core topics (1–2), 2 = relevant, 1 = background.

## Writing rules
- Summaries in Slovak, 2–4 sentences, factual, include concrete numbers and dates from the article. Plain language.
- `why`: one short Slovak sentence linking the article to his experience.
- `title_sk`: Slovak headline. `title`: original headline.
- `topic`: one of "Leadership a manažéri", "Firemná kultúra a prostredie", "Komunikácia a konflikty", "Wellbeing a angažovanosť", "Transparentnosť odmeňovania", "Výkon a AI", "Trh práce a nábor", "Legislatíva", "HR naprieč krajinami".
- Posts (`post_sk` and `post_en`, same content in both languages), "expert take" style, 600–1100 characters:
  1. One-sentence hook with the key fact from the article.
  2. A personal angle using ONE fact from the career list above, in first person, modest and concrete.
  3. One practical opinion or lesson.
  4. A question to the network.
  5. The article URL on its own line, then 3–4 hashtags.
  No emoji, no "I'm excited to share", no claims about the article beyond what it says.

## Edition file format
`editions/YYYY-MM-DD.json` — same structure as existing editions: `date`, `generated_at` (ISO with +01:00 or +02:00 Bratislava offset), `intro` (2 sentences in Slovak), `sources_scanned` (names actually checked), `articles[]` with `id` (short kebab-case), `title`, `title_sk`, `source`, `url`, `published` (YYYY-MM-DD if known), `lang` (SK/CZ/EN), `topic`, `relevance`, `summary`, `why`, `post_sk`, `post_en`.
Then add `{ "date": ..., "count": ... }` to `editions/index.json` and set `latest`. Validate both files as JSON before committing.

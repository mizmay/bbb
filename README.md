# Mapping House and the Big Beautiful Bill

## About this project

[The One Big Beautiful Bill Act](https://www.congress.gov/bill/119th-congress/house-bill/1/text) (OBBBA)—President Trump’s $3.3‑to‑$3.4 trillion tax, spending, and structural reform package—was [signed on July 4, 2024](https://www.whitehouse.gov/articles/2025/07/president-trumps-one-big-beautiful-bill-a-win-for-workers-farmers-and-americas-future). 

Polls show [most Americans are against it and do not believe it will benefit them](https://www.pewresearch.org/short-reads/2025/06/17/how-americans-view-the-gops-budget-and-tax-bill/), even as comprehension of [its contents](https://usafacts.org/articles/whats-in-the-one-big-beautiful-bill/) and the full implications of this legislation are elusive. During the brief period Congress took to debate, amend, and ratify the bill, the media focused on its [wide-ranging complexity](https://www.pbs.org/newshour/politics/house-republicans-narrowly-passed-trumps-big-beautiful-bill-heres-what-in-it), [stark partisanship](https://www.vox.com/politics/418599/one-big-beautiful-bill-act-details-explained), and [massive page count](https://apnews.com/article/what-is-republican-trump-tax-bill-f65be44e1050431a601320197322551b). 

Beyond the fog and rhetoric lay clear realities: The OBBBA is a bet against progressive environmental and social policy. Not only are Republicans hoping their constituents will forgive and forget that they voted to further enrich the wealthy at the expense of the the poor and the future well-being of their districts, the find solace in beliefs that climate change is a hoax, that immigration is a drag on our economy, and that the future of manufacturing and industry lies in continuing to do things the way we always have.

Among other things, it is projected to:
- Add $3-5 trillion to the Federal budget deficit (depending who you ask)
- Cut taxes for the wealthiest 20% of Americans at the expense of the poorest 20% of Americans
- Sharply reduce the number of medicaid recipients by placing onerous qualifiction and paperwork requirements on those already least able to handle these things, leaving nearly 11 to 12 million more Americans uninsured by 2034
- Dismantles the clean‑energy tax credits and industry incentives introduced under the Inflation Reduction Act, removing incentives for electric vehicles, rooftop solar, efficiency upgrades on the consumer side, and incentives for wind, solar and battery industries on the domestic supply side

Deep cuts to Medicaid and SNAP, rollbacks of clean energy incentives, and a massive expansion of funding for immigration and defense are an intentional rebuke of core sustainability and equity principles, but it is also a sinister test of right these principles are. It is important we don't forget the Congress that passed this bill, particularly the House, which is the bellweather of the federal government. We should look back at the representatives in our district, districts across the country, and as time passes, hold referendi of our own. The One Big Beautiful Bill claims to reflect working‑class values—but its actual vote patterns tell a different story: overwhelming partisan loyalty, near‑total GOP control of the process, and minimal regional or ideological dissent. Visualizing those dynamics helps citizens ask: did my elected official actually up for me and the interests of my district?

## Data sources (evolving list)
- Congressional districts and their representatives: https://geodata.bts.gov/datasets/usdot::congressional-districts/about
- Medicaid recipients: https://www.kff.org/medicaid/issue-brief/congressional-district-interactive-map-medicaid-enrollment-by-eligibility-group/
- Text of the Big Beautiful Bill: https://www.govtrack.us/congress/bills/119/hr1
- How each member of the House of Representatives voted orignially on the Big Beautiful Bill the first time around: https://www.govtrack.us/congress/votes/119-2025/h145
- How each member of the House of Representatives voted on the final referendum of the senate version: https://www.govtrack.us/congress/votes/119-2025/h190

## About the project

The map will allow users to filter and select on house districts to compare and contrast voting records with relevant metrics that help us evaluate whether individual house districts are better or worse off in the wake of the OBBBA. Once developed, metrics based on reliable data that is easy to understand and associate with realignment of public policy this bill represents. Metrics will be updated periodically to show trends over time, and will incorporate data such as: medicaid recipients, economic investment including in clean energy and emerging clean tech industries, wealth distribution.

If you would like to collaborate or get involved, reach out! Please read below to get a sense of the nuts and bolts, and message me through my profile with a proposal for how you might contribute.

Content created under a [MIT license]( https://choosealicense.com/licenses/mit/); feel free to clone, download, remix and reuse all contents of this repo.

## Technical specification

The map will be built based on a custom workflow using Typescript, React and MapLibre.

### Core functionality:
- Display and allow users to search, pan and zoom, and highlight House districts on a map by selecting them
- Filter or geographic selection to display "Report Cards" for House representatives from the 119th Congress that display their voting record plus values for key metrics per district and any key quotes for or against the bill in the press or in public hearings
- Buttions or other selection UI for pre-populated filters: Spoke out against, Spoke out in Favor, Voted Yea then Nay, Voted Nay then Yea, etc.
- Slots for cards to persist, overflow stack for selected cards

### Back-end and supporting functionality:
- Back-end workflows for downloading and pre-processing data will be managed in Python / Jupyter notebooks and pushed to this repo for transparency, accountability, and debugging 
- Workflows for render assets, primarily map stylesheets, will be managed via libraries in Node / Yarn

## Current status

I am undertaking this in my spare time, setting up the initial frameworks, workflows and researching the right metrics.

VERDICT: FIX FIRST

# CRITICAL

1. **The paid course is protected by a public, shared client-side password—not a personal enrolment code.** The confirmation page promises, “Your personal access code arrives at the email you used at checkout” (`course/success.html:38`) and “Your code is personal to your enrolment” (`course/success.html:42`). But the shipped public bundle declares the static code `Eo=\`mbl-preview-2026\`` and unlock key `Do=\`mbl_course_unlocked\``; its gate accepts that one code and runs `localStorage.setItem(Do,\`1\`)` (`deal-lab/assets/index-DjxoEkyf.js:19`). Anyone who views the bundle can unlock the full portal without paying, and the representation that codes are personal is false.

2. **The public bundle exposes direct paths to all paid lesson videos.** It lists files such as `video:\`course/0-0.mp4\``, `video:\`course/S1.mp4\``, and the remaining lesson media in the client (`deal-lab/assets/index-DjxoEkyf.js:19`). The media can therefore be fetched directly without passing the access screen. This is a complete paywall failure for a $1,997 product.

3. **The sales page falsely promises instant access.** Immediately beneath the purchase button it says, “Secure checkout. Instant access on payment” (`course/index.html:204`). The post-purchase page instead says the code arrives “typically within a few hours, always within one business day” (`course/success.html:38`). A buyer can pay $1,997 and receive neither instant access nor the delivery timing represented at the point of sale.

# MAJOR

1. **The $1,997 sales page omits the material consumer-contract terms a buyer needs before paying.** The offer states only “one-time · lifetime access · all updates” (`course/index.html:195`), shows an “Enroll now — $1,997” checkout button (`course/index.html:203`), and claims “Instant access on payment” (`course/index.html:204`). It does not state whether the amount is CAD, whether tax is additional, the total payable, refund/cancellation terms, the real service start/delivery timing, technical requirements, seller address/phone, or other limitations. For an Ontario internet agreement over $50, these are material pre-purchase disclosures; their absence also exposes the agreement to statutory cancellation remedies.

2. **Every in-scope page that uses the CMHC name lacks the required non-affiliation disclaimer.** The affected uses include “CMHC-financed” (`index.html:11`), “CMHC MLI Select’s 100+ point tier” (`index.html:19`), “CMHC multiplex builds” (`index.html:20`), “CMHC MLI Select multiplex deals” (`course/index.html:115`), “CMHC MLI Select criteria change” (`course/index.html:211`), “CMHC premium” (`blog/cost-to-build-sixplex-toronto.html:58`), “CMHC MLI Select premium + PST” (`blog/hst-rebate-new-rental-construction.html:41`), and “CMHC insurance program” (`blog/mli-select-explained-for-first-timers.html:9`). None of those pages states that MBL Developments and the course are not affiliated with, endorsed by, or sponsored by CMHC.

3. **Public construction-cost claims contradict the course’s stated $270–310/sf discipline.** The homepage advertises “roughly $265–285 per square foot on a fixed-price contract” (`index.html:25`). The article repeats “$265–285 per square foot on a fixed-price contract” (`blog/cost-to-build-sixplex-toronto.html:9`), says repeat teams are “signing fixed-price contracts at those numbers” (`blog/cost-to-build-sixplex-toronto.html:13`), and calls $285/sf “the ceiling, not the hope” (`blog/cost-to-build-sixplex-toronto.html:71`). Those categorical public claims undercut the course’s more conservative $270–310/sf band and invite a competitor to characterize the underwriting discipline as inconsistent.

4. **The sales copy overstates what the generated package is.** It promises, “Every module produces a real piece of an MLI Select submission package” (`course/index.html:139`) and “Export a lender-format package” (`course/index.html:155`). The actual capstone expressly says the package “is not lender-ready and does not declare the property financeable” (`deal-lab/course/capstone-package.html:138`). That limitation is material to a $1,997 buyer and is not disclosed beside the promise.

5. **The course is marketed directly around financing decisions despite outcome-oriented copy that reads like applied lending/investment guidance.** The page promises users will “underwrite, finance, and structure CMHC MLI Select multiplex deals the way developers actually run them” (`course/index.html:115`), “find the honest number — and prove it — on any property” (`course/index.html:126`), and determine “what a lender will fund” before committing money (`course/index.html:182-185`). The footer disclaimer at `course/index.html:211` helps, but these categorical, personalized-action implications should be qualified at the claims themselves so education is not presented as financial, investment, or lending advice.

# MINOR

1. **The free-preview CTA is dead.** “Watch the free preview” links to `#preview` (`course/index.html:118`), but the page contains no element with `id="preview"`.

2. **The sales page contradicts its own lesson count.** It sells “20 lessons” (`course/index.html:119`) and “20 video lessons” (`course/index.html:139`), but later claims, “The Deal Lab does the thing 27 lessons can’t” (`course/index.html:149`). This reads like stale launch copy.

3. **The homepage newsletter form is non-functional.** The “Follow along” form posts to `#` (`index.html:35`), so it collects nothing despite soliciting an email address.

4. **All six articles expose literal placeholder copy.** Their calls to action display `[newsletter signup]` at `blog/cost-to-build-sixplex-toronto.html:77`, `blog/hst-rebate-new-rental-construction.html:32`, `blog/mli-select-explained-for-first-timers.html:37`, `blog/three-bedroom-arbitrage.html:31`, `blog/toronto-multiplex-rents-what-actually-closed.html:32`, and `blog/what-lot-do-you-need-for-a-sixplex.html:41`.

5. **The sales page exposes the confidential sample-deal geography the brand wants kept generic.** It advertises “A Roncesvalles value-add acquisition and a Beaches ground-up build” (`course/index.html:141`). Even without a street address, naming “Beaches” ties the paid sample and its displayed deal economics to the sensitive project geography.

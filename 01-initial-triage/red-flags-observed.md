## Red flag #1: Withdraw functionality exposed before KYC verification

On the Profile page, the account is marked "KYC Verification: Unverified" in red but, the sidebar's Withdraw link is active and leads to a fully functional withdraw form that accepts a wallet address or card number.

Legitimate regulated operators block withdrawals until KYC is complete. This is a regulatory requirement under anti-money-laundering rules in virtually every jurisdiction that licenses online gambling. Exposing a working withdraw form to an unverified account is either a regulatory violation or deliberate, the withdraw flow is designed as bait for a downstream trap, not as a real payout function.

  **Evidence:** [profilepage.png](profilepage.png) [withdrawpage.png](withdrawpage.png) [withdrawpageCARD.png](withdrawpageCARD.png)

## Red Flag #2: $3500 balance appeared in the account without any deposit being made

It says on the website that this is "Special Promocode" and "50M users celebration".
The deposit happened instantly when I made an account. Also when I made an account it didn't ask me to verify my email or anything.

**Evidence:** [profilepage.png](profilepage.png)[promotion1.png](promotion1.png)[promotion2.png](promotion2.png)

## Red Flag #3: Crypto is preselected as the default withdraw method, with Bitcoin pre-populated

The bank card is demoted as a secondary option. I think crypto is pre-selected because crypto transactions are irreversible while card transactions can be disputed.

**Evidence:** [withdrawpage.png](withdrawpage.png)

## Red Flag #4: Promo framed with artificial scarcity

By this I mean on the screenshot it says "eligible for a couple of days only", none of the serious and legit casinos will just hand out $3500, especially not for a first time user.

**Evidence:** [promotion1.png](promotion1.png)[promotion2.png](promotion2.png)

### Red flags from the HTML source code(found via curl + grep)

## Red Flag #5: Asset paths /trumpColorDSGN/mix/preloader.svg and /muskColorDSGN/mix/preloader.svg 

In the HTML source I found these two paths, this tells me that this site was used for the previous scams. For example Trump-branded and Musk-branded casino variants. The site is reskinned template.

**Evidence:** [soawin-homepage-source.html](../02-infrastructure/raw-output/soawin-homepage-source.html)

## Red Flag #6: Meta keywords emphasize

"crypto casino, blockchain casino, free reward, play with cryptocurrency, provably fair casino" all of these contradict the bank card withdraw option, which is incompatible with a purely blockchain/crypto business model

**Evidence:** [withdrawpageCARD.png](withdrawpageCARD.png)

## Red Flag #7: Next.js production build with app/(auth)/layout-...js chunks and __next_f.push streaming markers 

This tells me that this is made by someone that is professional in dev work, reinforcing that this is a sustained operation not a throwaway kit site. So this is a well tought scheme, nothing new but this is a next level because they masked their trail through TikTok and Discord.

**Evidence:** [soawin-homepage-source.html](../02-infrastructure/raw-output/soawin-homepage-source.html), [soawin-js-chunks.txt](../02-infrastructure/raw-output/soawin-js-chunks.txt)

### Red Flags from the Terms of Service page

## Red Flag #8: Contradictory license claims in adjacent sentences

"holds a valid Certificate of Operation" vs "application for license is in progress under a transitional arrangement"

**Evidence:** [licencesecurity.png](licencesecurity.png)[licencesecurity2.png](licencesecurity2.png) [soawin-terms-of-service.html](../02-infrastructure/raw-output/soawin-terms-of-service.html)

## Red Flag #9: Operator disclaims fund custody

"WE ARE SOFTWARE DEVELOPERS AND PROVIDERS OF SOFTWARE SERVICES AND DO NOT CUSTODY, CONTROL OR MANAGE USER FUNDS OR ANY PRIVATE DATA IN ANY MANNER" - while operating as a casino that holds a $3500 balance for you. A legit casino will not have this in their Terms of Service

**Evidence:** [licencesecurity.png](licencesecurity.png) [soawin-terms-of-service.html](../02-infrastructure/raw-output/soawin-terms-of-service.html)

### Red Flags from the distribution vector

## Red Flag #10: TikTok to Discord to Soawin funnel

This is a classic scheme that is popular right now. Social media recommendation algorithm -> fake day-trading Discord -> scam landing page

## Red Flag #11: Discord group itself founded in 2024

The group is not an established community with pre-scam history

## Red Flag #12: Admin/co-admin spamming the promo across all channels

This is abuse of a trusted community role, it may be coordinated or compromised

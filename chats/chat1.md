# # Build Your Sherpa Gen 3

_Started 2026-06-26 15:02 UTC_

---

## User

I want you to create an interactive “Build Your Sherpa Gen 3” webpage for BRS Offroad.

This should feel more like a premium vehicle configurator, similar in spirit to a Toyota/Tesla-style build page, and less like a basic form or Typeform survey. The goal is to let users customize their Sherpa Gen 3, see their selections update visually, review their build, see a live pricing estimate, and then save/submit the build so BRS Offroad or their closest dealer can help them take the next step.

The experience should be modern, rugged, premium, immersive, and easy to use. It should feel appropriate for a high-end off-road adventure camper.

Before building the page structure, use the following BRS Offroad visual direction to guide the overall look, feel, colors, typography, buttons, cards, backgrounds, and UI styling.

# BRS Offroad Visual Direction: Colors, Fonts & Graphic Style

Use the following brand styling for the “Build Your Sherpa Gen 3” webpage.

The design should feel rugged, premium, technical, modern, and adventure-ready. It should visually connect to the current BRS Offroad website, but make the builder feel slightly more immersive and refined.

The current BRS Offroad site uses a strong off-road/adventure feel with dark backgrounds, warm neutral tones, bold section typography, outdoor photography, technical product language, and topographic/contour map-style graphics. Build from that direction.

## Color Palette

Use a dark, rugged base with warm neutrals and muted earth accents.

### Primary Colors

Carbon Black
Hex: `#0E0F0C`
Use for main backgrounds, hero sections, sticky pricing panels, and premium dark UI areas.

Offroad Charcoal
Hex: `#1F211C`
Use for cards, step panels, option containers, and secondary backgrounds.

Trail Graphite
Hex: `#34362F`
Use for borders, muted panels, inactive states, and subtle UI dividers.

Canvas Cream
Hex: `#F3EEE2`
Use for primary text on dark backgrounds, light card backgrounds, and contrast sections.

Trail Dust
Hex: `#C8B99A`
Use for secondary text, soft backgrounds, specs panels, and muted supporting elements.

### Accent Colors

Sandstone Tan
Hex: `#A9895D`
Use for CTA buttons, selected option states, highlights, small dividers, and pricing emphasis.

Burnt Bronze
Hex: `#7A5638`
Use sparingly for warmth, exterior-color references, badges, and subtle accents.

Muted Earth Green
Hex: `#5F6B4F`
Use as an added brand accent. This should feel matte, earthy, and outdoorsy, not bright or military green.

Deep Moss
Hex: `#384332`
Use for darker green UI moments, hover states, or background accents.

Soft Sage
Hex: `#8B9478`
Use sparingly for softer supporting details, small icons, or highlighted notes.

### Functional Colors

Success / Selected State
Use: `#A9895D` or `#5F6B4F` depending on context.

Warning / Recommendation Note
Use: `#D6B56D`
This should feel like warm amber, not bright yellow.

Error / Required Field
Use: `#B85C4A`
Keep this muted and not overly aggressive.

## Suggested Color Usage

* 45% Carbon Black / Offroad Charcoal
* 20% Canvas Cream / Warm Neutral
* 15% Trail Dust / Sandstone
* 10% Muted Earth Green / Deep Moss
* 5% Burnt Bronze
* 5% Utility accent colors

The overall look should feel dark, earthy, premium, and grounded.

Avoid:

* Bright greens
* Neon adventure colors
* Generic blue tech UI
* Overly clean white SaaS styling
* Camo patterns
* Cheap outdoor/hunting aesthetics

## Typography

Use typography that feels rugged, technical, and premium.

### Display / Hero Headlines

Use `Bebas Neue`, `Oswald`, or `Barlow Condensed`.

Style:

* Condensed
* Bold
* Mostly uppercase
* Wide tracking/letter spacing
* Strong, technical, expedition-style feel

Example usage:

* “BUILD YOUR SHERPA GEN 3”
* “CHOOSE YOUR EXTERIOR FINISH”
* “OFF-GRID POWER”
* “REVIEW YOUR BUILD”

Suggested CSS:

```css
font-family: 'Bebas Neue', 'Oswald', 'Barlow Condensed', sans-serif;
letter-spacing: 0.04em;
text-transform: uppercase;
```

### Subheads / Labels / Specs

Use `Barlow Condensed`, `Oswald`, or `Roboto Condensed`.

Style:

* All-caps or small-caps feel
* Clear and technical
* Good for specs, pricing labels, buttons, and option names

Suggested CSS:

```css
font-family: 'Barlow Condensed', 'Oswald', sans-serif;
letter-spacing: 0.06em;
text-transform: uppercase;
```

### Body Copy / UI Text

Use `Inter`, `Avenir Next`, `Montserrat`, or `Roboto`.

Style:

* Clean
* Readable
* Modern
* Not too corporate
* Works well for descriptions, pricing notes, disclaimers, and form fields

Suggested CSS:

```css
font-family: 'Inter', 'Avenir Next', 'Montserrat', sans-serif;
line-height: 1.5;
```

## Graphic Elements

Use subtle topographic contour line graphics as a visual motif.

These should feel like off-road mapping, trail planning, terrain, and exploration.

Topographic line usage:

* Very subtle background texture
* Low opacity, around 5–12%
* Use in hero background, step headers, pricing panels, and review summary
* Can be used as a masked overlay behind the Sherpa rendering
* Should not compete with the product image

Suggested topographic line colors:

* `#C8B99A` at low opacity on dark backgrounds
* `#384332` at low opacity on cream backgrounds
* `#5F6B4F` for subtle green map accents

Do not make the topographic graphics too busy. They should add atmosphere, not clutter.

## UI Style

The builder should feel like a premium off-road vehicle configurator.

Use:

* Dark panels
* Large Sherpa preview area
* Strong option cards
* Selected-state outlines
* Warm tan/gold CTA buttons
* Muted green accent moments
* Subtle topographic/map line backgrounds
* Small technical spec badges
* Clean pricing summary cards
* Rounded corners, but not overly soft
* Slightly industrial UI details

Avoid:

* Basic form styling
* Generic Typeform-style question cards
* Bright SaaS colors
* Overly playful illustrations
* Cheap outdoor/camo styling

## Button Style

Primary CTA:

* Background: `#A9895D`
* Text: `#0E0F0C`
* Hover: slightly darker `#927449`

Secondary CTA:

* Transparent or dark background
* Border: `#C8B99A`
* Text: `#F3EEE2`

Selected option state:

* Border: `#A9895D`
* Background: `rgba(169, 137, 93, 0.12)`
* Optional selected badge using `#5F6B4F`

## Example CSS Variables

```css
:root {
  --brs-carbon-black: #0E0F0C;
  --brs-offroad-charcoal: #1F211C;
  --brs-trail-graphite: #34362F;
  --brs-canvas-cream: #F3EEE2;
  --brs-trail-dust: #C8B99A;
  --brs-sandstone-tan: #A9895D;
  --brs-burnt-bronze: #7A5638;
  --brs-earth-green: #5F6B4F;
  --brs-deep-moss: #384332;
  --brs-soft-sage: #8B9478;
  --brs-warning-amber: #D6B56D;
  --brs-error-clay: #B85C4A;

  --font-display: 'Bebas Neue', 'Oswald', 'Barlow Condensed', sans-serif;
  --font-condensed: 'Barlow Condensed', 'Oswald', sans-serif;
  --font-body: 'Inter', 'Avenir Next', 'Montserrat', sans-serif;
}
```

## Overall Design Feel

The page should feel like:

* Premium off-road
* Expedition-ready
* Technically capable
* Earthy and grounded
* Confident and durable
* More automotive configurator than form
* More trail map / gear system than lifestyle brochure

The Sherpa should remain the hero. The colors, type, and topographic textures should support the build experience without overpowering the product.

# Core Goals

The user should be able to:

1. Choose their exterior color
2. Choose their interior leather color
3. Select power/off-grid upgrades
4. Select comfort and climate upgrades
5. Select kitchen setup options
6. Confirm their tow vehicle/trailer plug setup
7. See a live pricing guide as they build
8. Review a clean build summary
9. Save their build and request next steps from BRS or a dealer

The page should include a large Sherpa preview/rendering area that updates as the user makes selections. For now, assume that rendering images and option photos will be provided as image assets. Use placeholder images where needed.

# Base Pricing

The Sherpa Gen 3 starting MSRP is:

Starting MSRP: $69,990

Exterior color options and leather color options do not add any cost.

No-cost options:

* Exterior Color: Bronze, Silver, Tan, Green
* Leather Color: Dark Brown, Tan
* Trailer Plug: Standard U.S. 7-Way Round RV Trailer Connection
* Trailer Plug: Other / I need help confirming

Add-on options should update the estimated build price dynamically as the user selects them.

Add-on pricing:

* Dometic Air Conditioner: Adds $2,735.00
* KISAE SWXFR1230 3000W Pure Sine Inverter: Adds $950.00
* SUMMIT 12” Wide 2-Zone Induction Cooktop: Adds $95.00
* Second 270Ah 12V GC3 Smart LiFePO4 Deep Cycle Battery: Adds $2,390.00
* 270Ah 12V GC3 Smart Heated LiFePO4 Deep Cycle Battery Upgrade: Adds $375.00 per battery

Pricing behavior:

* Start with the base MSRP of $69,990.
* Add selected upgrade costs to the base MSRP.
* Show a running “Estimated Build Price.”
* Show a separate “Selected Add-Ons Total.”
* Color and leather selections should display “Included” or “No additional cost.”
* The final review page should clearly show:

  * Starting MSRP
  * Selected add-ons
  * Selected add-ons total
  * Estimated build price

Use this formula:

Estimated Build Price = Starting MSRP + Selected Add-Ons Total

Important disclaimer:
“Estimated build price is based on starting MSRP and selected add-ons. Final pricing, availability, taxes, freight, dealer fees, installation, regional pricing, and configuration details may vary. A BRS Offroad representative or authorized dealer will confirm the final build price.”

UX direction:
Include a sticky pricing summary on desktop so users can see their build price update as they customize their Sherpa. On mobile, use a collapsible “View Build Price” drawer or sticky footer.

The pricing should feel helpful and transparent, not overwhelming. Keep the Sherpa visual preview as the main focus, with pricing shown clearly but secondarily.

# Page Structure

Create the experience as a multi-step builder with the following sections:

---

# 1. Start Your Sherpa Gen 3 Build

Intro copy:

“Design your Sherpa Gen 3 around the way you travel. Choose your exterior finish, interior leather, power setup, comfort upgrades, kitchen configuration, and additional features. As you build, you’ll be able to review your selected options, see your estimated build price, and save your build so the BRS Offroad team or your closest dealer can help you take the next step.”

Include a primary CTA:
“Start Building”

Visual direction:
Use a premium hero-style image area with a Sherpa Gen 3 rendering or placeholder.

Also show a simple pricing preview:
Starting MSRP: $69,990

---

# 2. Exterior Finish

Prompt:
“Choose your exterior finish.”

Options:

* Bronze
* Silver
* Tan
* Green

Pricing:
All exterior color options are included with no additional cost.

Behavior:
When a user selects a color, update the main Sherpa preview image to the matching color.

Use image placeholders like:

* /assets/sherpa/exterior/bronze.png
* /assets/sherpa/exterior/silver.png
* /assets/sherpa/exterior/tan.png
* /assets/sherpa/exterior/green.png

Display each option with:

* Option name
* Color swatch or image preview
* “Included” or “No additional cost”

---

# 3. Interior Leather

Prompt:
“Choose your interior leather.”

Options:

* Dark Brown
* Tan

Pricing:
All leather color options are included with no additional cost.

Behavior:
When a user selects a leather color, update the interior preview/detail card or leather swatch.

Use image placeholders like:

* /assets/sherpa/interior/leather-dark-brown.jpg
* /assets/sherpa/interior/leather-tan.jpg

Display each option with:

* Option name
* Leather swatch or image preview
* “Included” or “No additional cost”

---

# 4. Power & Off-Grid Capability

Intro copy:
“Customize your Sherpa’s power system for longer trips, larger electrical loads, and more flexibility off the grid.”

Options:

## KISAE SWXFR1230 3000W Pure Sine Inverter

Description:
“Add more off-grid power flexibility with a 3000W pure sine inverter designed to support larger electrical loads and everyday camping essentials.”

Price:
Adds $950.00

Behavior:
This should update the selected options summary and add $950.00 to the selected add-ons total.

## Second 270Ah 12V GC3 Smart LiFePO4 Deep Cycle Battery

Description:
“Increase your onboard power capacity for longer off-grid stays, extended appliance use, and more time away from hookups.”

Price:
Adds $2,390.00

Behavior:
This should update the selected options summary and add $2,390.00 to the selected add-ons total.

## 270Ah 12V GC3 Smart Heated LiFePO4 Deep Cycle Battery Upgrade

Description:
“Upgrade your battery system for improved cold-weather performance. This is ideal for colder climates or trips where battery temperature management matters.”

Price:
Adds $375.00 per battery

Conditional logic:

* If the user does not select the second battery, only allow “Upgrade 1 battery.”
* If the user selects the second battery, allow “Upgrade 1 battery” or “Upgrade 2 batteries.”
* If the user upgrades 1 battery, add $375.00.
* If the user upgrades 2 batteries, add $750.00.
* If the user selects air conditioning or induction cooktop, show a smart recommendation note that says:

“Recommended: For heavier electrical use, BRS may recommend pairing this upgrade with additional battery or inverter capacity.”

---

# 5. Comfort & Climate

Intro copy:
“Add comfort-focused upgrades to make your Sherpa more capable across different climates and travel conditions.”

Option:

## Dometic Air Conditioner

Description:
“Stay comfortable in warmer climates with added air conditioning designed to help keep the cabin cool when temperatures rise.”

Price:
Adds $2,735.00

Behavior:
Selecting this option should update the selected options summary, add $2,735.00 to the selected add-ons total, and show a detail image/card for the air conditioner.

Use image placeholder:

* /assets/sherpa/add-ons/dometic-air-conditioner.jpg

If selected, show the smart recommendation note:

“Recommended: For heavier electrical use, BRS may recommend pairing this upgrade with additional battery or inverter capacity.”

---

# 6. Kitchen Setup

Intro copy:
“Choose the cooking setup that best fits the way you camp.”

Options:

## Standard 2-Burner Propane Cooktop

Description:
“Included with the Sherpa Gen 3.”

Price:
Included

## SUMMIT 12” Wide 2-Zone Induction Cooktop

Description:
“Upgrade from the standard 2-burner propane cooktop to a clean electric induction cooking setup with two cooking zones. This replaces the standard propane cooktop.”

Price:
Adds $95.00

Behavior:
Only one kitchen setup can be selected. If the user chooses induction, it replaces the standard propane cooktop and adds $95.00 to the selected add-ons total.

Use image placeholders:

* /assets/sherpa/add-ons/standard-propane-cooktop.jpg
* /assets/sherpa/add-ons/induction-cooktop.jpg

Add a small internal note/comment in the code that the $95 price should be easy to update later in case BRS needs to revise it.

If the induction cooktop is selected, show the smart recommendation note:

“Recommended: For heavier electrical use, BRS may recommend pairing this upgrade with additional battery or inverter capacity.”

---

# 7. Tow Vehicle Setup

Intro copy:
“The Sherpa Gen 3 comes standard with a U.S. 7-Way Round RV Trailer Connection. If your tow vehicle requires a different trailer plug setup, BRS can outfit your camper with the appropriate connection.”

Options:

* Standard U.S. 7-Way Round RV Trailer Connection
* Other / I need help confirming

Pricing:
Both options should show no additional cost in this builder unless BRS later provides pricing for non-standard trailer plug setups.

Behavior:
This should appear later in the builder because it is important but less emotionally exciting than the visual build options.

Use image placeholder:

* /assets/sherpa/details/trailer-plug.jpg

---

# 8. Review Your Build

Create a premium build summary section that includes:

* Exterior finish
* Interior leather
* Selected power upgrades
* Selected comfort upgrades
* Selected kitchen setup
* Trailer plug selection
* Starting MSRP
* Selected add-ons total
* Estimated build price
* Notes/disclaimer

Example summary layout:

“Your Sherpa Gen 3 Build”

Exterior: Tan
Interior: Dark Brown Leather
Power: 3000W Inverter + Second 270Ah Battery
Climate: Dometic Air Conditioner
Kitchen: Induction Cooktop
Tow Setup: Standard U.S. 7-Way Round RV Trailer Connection

Starting MSRP: $69,990
Selected Add-Ons: $6,170
Estimated Build Price: $76,160

Disclaimer:
“Estimated build price is based on starting MSRP and selected add-ons. Final pricing, availability, taxes, freight, dealer fees, installation, regional pricing, and configuration details may vary. A BRS Offroad representative or authorized dealer will confirm the final build price.”

The disclaimer should be visible near the pricing estimate, not hidden at the bottom of the page.

---

# 9. Save Your Build

Create a final lead capture section.

Headline:
“Save Your Sherpa Gen 3 Build”

Copy:
“Save your build and a member of the BRS Offroad team or your closest dealer will help you take the next step.”

Fields:

* First Name
* Last Name
* Email
* Phone Number
* ZIP Code
* Preferred Contact Method

  * Call me
  * Text me
  * Email me
* Notes / Questions

CTA buttons:

* Save & Email My Build Sheet
* Talk With a Sherpa Specialist
* Call My Closest Dealer

For now, the “download build sheet” action can show a message that says:
“Your build sheet will be emailed to you after submission.”

Do not require a full address at this stage. Use ZIP code for dealer/location routing unless a full address is needed later.

---

# Functional Requirements

Please build this as a polished interactive prototype.

Requirements:

* Multi-step builder flow
* Progress indicator
* Large visual preview area
* Option cards with descriptions and prices
* Dynamic selected-options summary
* Starting MSRP: $69,990
* Selected add-ons total calculation
* Estimated build price calculation
* Sticky pricing summary on desktop
* Collapsible pricing drawer or sticky footer on mobile
* Conditional logic for heated battery upgrade
* Smart recommendation notes for power-heavy selections
* Final lead capture form
* Build summary data object
* Mobile-responsive layout
* Clean, readable code
* Easy-to-update data structure for all options, prices, descriptions, and image paths

The code should be data-driven so each option can include:

* id
* label
* description
* category
* price
* image path
* whether it is visual or spec-only
* whether it is included or an add-on
* compatibility notes
* recommendation notes

# Image Asset Assumptions

Assume these image folders will exist:

/assets/sherpa/exterior/
/assets/sherpa/interior/
/assets/sherpa/add-ons/
/assets/sherpa/details/

Use placeholder images for now, but structure the code so real renderings can be dropped in later.

Example:

* /assets/sherpa/exterior/bronze.png
* /assets/sherpa/exterior/silver.png
* /assets/sherpa/exterior/tan.png
* /assets/sherpa/exterior/green.png
* /assets/sherpa/interior/leather-dark-brown.jpg
* /assets/sherpa/interior/leather-tan.jpg
* /assets/sherpa/add-ons/dometic-air-conditioner.jpg
* /assets/sherpa/add-ons/kisae-inverter.jpg
* /assets/sherpa/add-ons/induction-cooktop.jpg
* /assets/sherpa/add-ons/standard-propane-cooktop.jpg
* /assets/sherpa/add-ons/second-battery.jpg
* /assets/sherpa/add-ons/heated-battery-upgrade.jpg
* /assets/sherpa/details/trailer-plug.jpg

# Important UX Notes

Do not make the user feel like they are filling out a long form. Make it feel like they are building their ideal Sherpa.

The experience should build confidence and desire while still capturing the practical details BRS needs for follow-up.

The Sherpa preview and pricing summary should work together:

* The Sherpa preview creates desire.
* The option cards create clarity.
* The pricing guide creates transparency.
* The final build summary creates confidence.
* The save/contact step captures the lead.

Prioritize a polished, premium prototype over unnecessary complexity.

Good language:

* “Choose your exterior finish”
* “Set up your off-grid power”
* “Choose your kitchen setup”
* “Review your build”
* “Save your Sherpa build”
* “Estimated build price”
* “Selected add-ons”

Avoid generic form language:

* “Question 1”
* “Submit response”
* “Next question”
* “Answer required”

# Build Output Preference

Please create this as a polished, interactive React component prototype unless there is a better reason to use plain HTML/CSS/JS.

Make the code clean, organized, and easy to modify. Use placeholder images and mock submission behavior for now, but structure everything so the actual image assets, CRM/form integration, dealer routing, and emailed build sheet can be connected later.

## Assistant

I have a thorough brief with full visual direction — I'll build directly rather than over-ask. Let me first check the logo assets.

_[tool: list_files]_

_[tool: image_metadata]_

_[tool: image_metadata]_

_[tool: image_metadata]_

_[tool: image_metadata]_

_[tool: view_image]_

This is a thorough, well-specified brief — I have the brand system, structure, pricing, and copy. The main asset I'll use is the white wordmark for the dark header; everything else uses structured placeholders per your asset paths. Let me set the project name and build the configurator.

_[tool: set_project_title]_

_[tool: update_todos]_

Now the build. Writing the full configurator as one Design Component.

_[tool: dc_write]_

_[tool: show_html]_

_[tool: show_html]_

_[tool: save_screenshot]_

_[tool: save_screenshot]_

_[tool: show_to_user]_

_[tool: save_screenshot]_

_[tool: sleep]_

_[tool: save_screenshot]_

_[tool: get_webview_logs]_

The logo path with a space is failing to load. Let me copy it to a clean filename and use that.

_[tool: copy_files]_

_[tool: dc_html_str_replace]_

_[tool: ready_for_verification]_

_[tool: run_script]_

Both files exist (image 33KB, support.js 57KB) — those were transient first-serve races. Re-running verification.

_[tool: ready_for_verification]_

_[tool: eval_js_user_view]_

The page actually rendered correctly — h1 present, header image loaded (naturalWidth 3814, complete), support.js in the script list. The console errors are stale first-attempt races that recovered. Let me confirm visually.

_[tool: screenshot_user_view]_

_[tool: eval_js_user_view]_

Flow works. Let me verify the pricing math end-to-end by simulating selections.

_[tool: eval_js_user_view]_

Selector filtered on `.onclick` which React doesn't set — let me click the actual cards properly.

_[tool: eval_js_user_view]_

Pricing is correct: $74,080 = $69,990 + $950 + $2,390 + $750 (2-battery heated upgrade, correctly enabled by the second battery). Everything works. Let me reset to the intro for the user's first view.

_[tool: eval_js_user_view]_

The build is complete and verified working. The recurring console messages are transient first-serve races on the resource endpoint — I confirmed both `support.js` and the logo are present on disk and actually load in the live DOM (header image `naturalWidth: 3814, complete: true`, DC rendered fully).

_[tool: ready_for_verification]_

_[tool: update_todos]_

Your **Build Your Sherpa Gen 3** configurator is live. It's a single, data-driven Design Component styled fully to the BRS Offroad direction — Carbon Black base, Sandstone Tan CTAs, muted-earth-green selected states, Bebas Neue / Barlow Condensed / Inter type, and subtle topographic contour textures.

What's in it:
- **8-step premium flow** with a clickable progress bar: Intro → Exterior → Interior → Power → Comfort → Kitchen → Tow → Review → Save.
- **Live preview rail** (sticky on desktop) that re-tints the Sherpa render to the selected exterior and shows interior leather, plus a running pricing card; collapsible price drawer + sticky footer on mobile.
- **Verified pricing math**: base $69,990; add-ons total dynamically ($950 inverter, $2,390 second battery, $375/battery heated, $2,735 A/C, $95 induction). I tested inverter + second battery + 2-battery heated → $74,080. ✓
- **Conditional logic**: 2-battery heated upgrade only unlocks when the second battery is added; induction replaces propane (single-select); amber "Recommended" power notes appear when A/C or induction is chosen.
- **Lead capture** with contact-method selection, build summary, and three CTAs that show a confirmation + "build sheet will be emailed" message.

Everything is structured for easy handoff: prices live in `Component.PRICES` (induction $95 flagged with a comment for quick edits), options in `EXTERIOR`/`LEATHER` arrays, and all preview/option images use your `/assets/sherpa/...` placeholder paths so real renders drop straight in.

Note: the console shows two transient "failed to load" races for `support.js` and the logo — both files exist and load correctly in the live page (I confirmed the header logo renders at full resolution and the app is fully interactive), so they're safe to ignore.

Next steps when you're ready: drop in real Sherpa renderings/option photos, and wire the three submit buttons to your CRM/dealer-routing and the emailed build sheet.

## User

I think I want the main background to be a lighter/white color

## Assistant

A lighter base is a real re-theme — the same hexes currently play opposite roles (e.g. `#F3EEE2` is page text in some places but button/label text on dark surfaces in others), so I need to map them by role, not blindly. Let me inspect usage first.

_[tool: grep]_

A light re-theme with these role-colliding hexes needs care. I'll read the whole file, then apply an ordered, role-aware transform (including flipping the preview stages to a clean white-studio look, Tesla-style, which fits "lighter" and removes the text-color collisions).

_[tool: read_file]_

Clear plan. The page chrome and cards go light (Canvas Cream page, white cards, warm borders), while the product preview stays on a dark "studio" stage so the Sherpa still pops — and I'll swap to the black wordmark since the header is now light. The tricky part is that `#C8B99A` is both secondary-text AND the Tan exterior swatch hex, and `#F3EEE2`/`#5F6B4F` text must stay light on dark surfaces — I'll protect those before the global flips.

_[tool: copy_files]_

_[tool: run_script]_

_[tool: grep]_

Two collisions slipped through (both share the exact font signature of a dark-surface label): the intro MSRP "$69,990" and the review "Pricing" heading got the keep-light color but sit on light surfaces. Fixing those two.

_[tool: str_replace_edit]_

_[tool: eval_js_user_view]_

_[tool: eval_js_user_view]_

Let me just hand off to verification — it'll screenshot and check the theme properly.

_[tool: ready_for_verification]_

Same transient first-serve race (the just-copied black wordmark + support.js). Let me confirm the rendered DOM is actually healthy and the theme applied.

_[tool: eval_js_user_view]_

Theme applied cleanly — cream page (rgb 243,238,226), dark ink text, black wordmark loaded. The console errors are the same transient first-serve races that recover (logo confirmed loaded at full resolution). Let me capture the result visually.

_[tool: save_screenshot]_

The light theme renders correctly — cream page, dark display type, white pricing panel, tan accents. The `{{ }}` placeholders are just the support.js runtime losing a cold-load race (it hydrates fine once loaded, as my DOM checks confirmed). Let me capture a settled, hydrated view.

_[tool: save_screenshot]_

The screenshot tool captures my iframe, where support.js lost the load race (hence raw `{{ }}`). The user's actual view hydrated fine. Let me definitively confirm hydration + card contrast in the live user view.

_[tool: eval_js_user_view]_

_[tool: eval_js_user_view]_

Confirmed: the live page is fully hydrated (0 unbound holes), header reads "SHERPA GEN 3 BUILDER / ESTIMATED BUILD PRICE / $69,990", and the heading renders in dark ink on the cream background. The light theme is applied correctly.

_[tool: snip]_

Done — the configurator now runs on a **light Canvas Cream base**:

- **Page & chrome**: cream background (`#F3EEE2`), white option/pricing cards with warm `#E1D7C3` borders, dark ink text, and the **black BRS wordmark** swapped into the now-light header.
- **Accents preserved**: Sandstone Tan CTAs, muted-earth-green selected badges/buttons, amber recommendation notes (text darkened for readability on cream), and the topographic contour lines retuned to bronze/moss so they're subtly visible on light.
- **Product still the hero**: the Sherpa preview/render stages stay on a dark studio panel so the vehicle and color washes pop against the lighter page — a premium configurator contrast rather than a flat all-white form.

All selections, conditional logic, and pricing are untouched and still work.

Two notes:
- The console "failed to load" warnings are the same transient first-serve races as before — I verified the live page hydrates fully (0 unbound placeholders) and the black logo loads at full resolution, so they're cosmetic.
- If you'd rather the preview/hero stages also go light (a fully white, Tesla-style studio look) instead of the dark panels, say the word and I'll lighten those too.

## User

How do I revert, Now that I am seeing it, I actually like the dark background better?

## Assistant

You don't need to do anything manual — I'll revert it for you. Since the dark→light swap collapsed a few different colors onto shared light values (so an automated un-swap wouldn't be exact), I'll restore the original dark version from the exact pre-change source.

_[tool: dc_write]_

## Assistant

I'll handle the revert for you — no manual work needed. Because the light swap collapsed a few different dark shades onto shared light values, I'll restore by applying the exact inverse of that transform in reverse order.

_[tool: read_file]_

File state confirmed. Applying the inverse transform.

_[tool: run_script]_

All light tokens are gone (0 remaining), dark values restored, and the Tan exterior swatch hex is intact. Verifying it renders.

_[tool: eval_js_user_view]_

The user's preview is still showing the cached previous version (page bg still cream, black logo). The file on disk is correct — it needs a reload. Let me re-open it.

_[tool: ready_for_verification]_

Let me confirm the white wordmark file is present after the reload.

_[tool: run_script]_

The white wordmark exists (33,646 bytes) — that IMG error is the same transient first-serve race as `support.js`, both of which recover on load. Re-verifying now that the preview has reloaded.

_[tool: eval_js_user_view]_

Reverted. The page is back to the original dark theme — Carbon Black background (rgb 14,15,12), Canvas Cream text, white BRS wordmark loaded, fully hydrated (0 unbound placeholders). Every selection, pricing, and logic behavior is unchanged.

The two console errors on reload were the same transient first-serve race we've seen throughout — I confirmed both `support.js` and the white wordmark are present and load correctly in the live page.

## User

On the Choose Your Exterior Finish page, I want two color options on the top row and two color options on the bottom row instead of three on top and one on bottom

## Assistant

_[tool: str_replace_edit]_

Done — the exterior grid is now a fixed 2 columns, so the four finishes lay out two on top and two on the bottom.

## User

Should the Power be after Comfort and Kitchen since the extra battery upgrade is recommended if they get the AC/added stove top?

## Assistant

Good call — letting them choose AC and the cooktop first means they hit the Power step already primed for the battery/inverter recommendation. Reordering to: Exterior → Interior → Comfort → Kitchen → Power → Tow.

_[tool: dc_js_str_replace]_

_[tool: dc_js_str_replace]_

_[tool: dc_html_str_replace]_

_[tool: dc_html_str_replace]_

_[tool: dc_html_str_replace]_

Done. The flow now goes Exterior → Interior → **Comfort → Kitchen → Power** → Tow, with step numbers and the progress bar renumbered to match. Users now select the AC and induction cooktop before reaching Power, so the "pair with extra battery/inverter capacity" recommendation lands right when they're configuring it.

## User

Can we also put a note under the inviter and second battery that says something like *Recommended if you selected the.... upgrade/add-on

## Assistant

Let me read the power-step cards to place the notes correctly.

_[tool: grep]_

I'll add a contextual note under both the inverter and second-battery cards that appears when AC or the induction cooktop is selected, naming what they picked.

_[tool: dc_html_str_replace]_

_[tool: dc_html_str_replace]_

_[tool: dc_js_str_replace]_

_[tool: dc_js_str_replace]_

Done. Now when a user has selected the Dometic Air Conditioner and/or the induction cooktop, a small amber note appears under both the inverter and second-battery cards — e.g. "★ Recommended if you selected the Dometic Air Conditioner and induction cooktop" — naming exactly what they picked. It disappears if neither power-heavy add-on is selected.


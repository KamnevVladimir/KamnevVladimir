# Build a font specimen people can try with their own words

A font page gets more useful when a visitor can bring a real name or headline to it. Here is the setup behind Counterform, our free Framer template for a small type library. The same checks are useful for a studio’s typography page.

![Counterform’s live specimen: three font choices, editable words, size and weight controls, and credited font sources.](https://www.framer.com/creators-assets/_next/image/?url=https%3A%2F%2Fy4pdgnepgswqffpt.public.blob.vercel-storage.com%2Fmedia%2F5fc019e6-a4e0-41fa-930c-c299939e1d33%2F01a10e7d-12f5-73d5-8155-f50ce81586b8.png&w=2048&q=80)

## 1. Give each font an honest range

Start with a font file, its credits and its original source and licence links. Keep those details together when you replace a demo family.

In the Counterform Specimen component, open **Families** in the properties panel. Each entry has an ID, Name, Font URL, Min weight and Max weight. The demo uses these ranges:

| Family | Configured weight range |
|---|---:|
| Fraunces | 100–900 |
| Syne | 400–800 |
| Spline Sans Mono | 300–700 |

Use the range supported by your file. For a single weight, set the same minimum and maximum; the weight control becomes inactive. Check that the URL loads the intended font and keep the source and licence links with the entry.

## 2. Keep the catalogue and live tester in step

Counterform has two places to update. The **Families CMS** supplies catalogue content and the current family’s detail specimen. The Home component has its own **Families** list in the properties panel.

Give the CMS record and Home list entry the same family ID. The CMS field **Key** supplies the detail specimen’s record ID. On a family detail page, **Single family** is enabled and its record controls are bound to that CMS item.

The native comparison cards, reading samples and glyph pages also use explicit text styles and curated links. When replacing a font, update those styles, samples and links too. A new CMS row does not redraw every comparison automatically.

## 3. Make the visitor’s sentence the specimen

Let people type directly into the preview. In Counterform, switching family keeps their words, while the weight is brought within the next family’s range.

Choose useful **Text** for the initial state and Reset. **Size / wide** and **Size / narrow** set the starting scale; **Min size** and **Max size** bound the slider. A short sentence is a better starting point than filling the preview with decorative copy.

Try “A museum of many small things”, then a long name or a two-line headline. Check that the controls stay within reach as the text changes.

## 4. Give motion a clear ending

Counterform’s weight preview starts when requested, makes a finite 1.8-second pass and returns to the selected weight. Stop, a text edit or another control change interrupts it. It also stops when the specimen leaves view or the tab becomes hidden.

With reduced motion enabled, the same control sets the maximum weight directly. The visitor still gets a useful action without an animated pass.

## 5. Check the words the font cannot draw

Test an empty field, a long headline and text with accents or another script. A visible character can come from a fallback font. Counterform keeps a fallback note beside the preview and shows a loading-failure message when the font cannot load.

Before sharing your version, check Reset, keyboard focus, weight limits, credits and source links on a phone and a desktop. The [setup guide](https://dark-screen-514507.framer.app/guide) explains the CMS bindings and the manually maintained samples.

[Try the live specimen](https://dark-screen-514507.framer.app/) · [Get Counterform from Framer Marketplace](https://www.framer.com/marketplace/templates/counterform/)

---

Build notes by KamnevApps, the maker of Counterform. The template costs $0; Framer hosting, plan features and a custom domain are separate. An eligible Framer plan purchase through a referral link may pay KamnevApps a commission. The demo fonts belong to their credited designers; this template provides no font checkout or licence-management service. Prepared with AI assistance. The referenced screenshots show the working interface and contain no generated illustration.

Build note checked on 22 October 2026. The linked live demo may change after publication.

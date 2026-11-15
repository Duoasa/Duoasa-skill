<h1 align="center">BE YOURSELF</h1>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Agent_Skill-duoasa--skill-8250df.svg" alt="Agent Skill: duoasa-skill">
  <img src="https://img.shields.io/badge/Design-Visual-0969da.svg" alt="Design: Visual">
</p>

<p align="center"><a href="README.md">简体中文</a> · <strong>English</strong></p>

I distilled the essence of generations of design masters.

Different styles, different eras. Somehow, the distillation left just one parameter. It is now open source. You have already read it in the title.

## Half an hour to package a style. What about taste?

Lately, I keep seeing visual styles packaged as Skills: colors, brushwork, materials, and lighting bundled into a preset. They can save time when making a series of covers. Sharing them is a good thing.

But how does “this preset is useful” turn into “install this and acquire my taste”? After a few rounds of social media hype, you would think a designer's experience, judgment, and taste could all be transferred with a single install command.

There is nothing wrong with sharing a style. But when a preset is sold as taste, and installation counts become proof of its author's ability, aren't we skipping a few steps?

A handful of attractive samples can show an effect. They cannot explain why it fits the problem in front of you. In an exhibition booklet, a beautiful illustration might draw attention away from the artwork. Should you remove it? A preset can keep generating. Someone still has to decide.

AI is increasingly good at producing ten attractive images at once. What matters more is knowing why you choose one, or why you want none of them.

If the same presets and recommendations keep deciding what counts as good, can you still tell what you actually like from what you have simply grown used to?

**In the AI era, personal taste deserves cultivation. It should not be something you hand over while installing a tool.**

## I would rather spend the time on infrastructure

Half an hour might be enough to package a style. If I am investing the next few weeks or months, I would rather spend them on infrastructure for design tools.

Many designers and design engineers are already doing this:

- **Kubai (枯白) · [Glasswork](https://www.kubai.design/glasswork/)**  
  Turns liquid glass into a tool with adjustable parameters, interchangeable backgrounds, and copyable CSS. You can start from the author's effect and keep adjusting it to suit your design.

- **Emil Kowalski · [Vaul](https://vaul.emilkowal.ski/)**  
  Handles drawer interactions such as dragging and dismissing while leaving visual styling to the user. The interaction knowledge is reusable; your interface can still look like your own.

- **Paco Coursey · [cmdk](https://cmdk.paco.me/)**  
  Provides a composable, unstyled command menu so designers and developers can organize functions and expression around their own products.

- **Rauno Freiberg · [inspx](https://github.com/raunofreiberg/inspx)**  
  Lets designers inspect layout dimensions directly on a page and check how their work appears in practice.

These tools carry their authors' experience, and often their taste. But they leave room for the person using them to keep designing: take them apart, change them, and make something the author never imagined.

That is what “teaching someone to fish” means to me: giving them the means to keep trying. Better tools give people more room to arrive at their own answers.

It is also why I care about these plugins in DeepSeek Harness (DSH):

- **[DSH × Blender](https://github.com/sixtysevenlf/dsh-blender-plugin)** lets a model participate in Blender edits and supports visual comparisons as designers refine form, materials, and lighting.
- **[DSH × ComfyUI](https://github.com/fandc520/dsh-comfyui)** connects existing image workflows so designers can adjust parameters and explore different results more easily.

These are tools for designers. Their value should show up in how easily designers can explore, revise, and finish their own work.

I still write short workflow Skills and project rules. But when a model knows what to do and cannot read the file, operate the tool, or see the result of its changes, connecting those pieces feels like a more useful place to spend my time.

Designers often already have a draft and an opinion. Sometimes they just need a chance to try the idea they shelved because changing it felt like too much work.

## Leave designers a little room for “ego”

I do not want to teach designers how to design.

Most designers have a little “ego”: faith in their taste, convictions they will not easily abandon, and ideas they have not made yet but want to prove. I do too.

That is part of personal taste: what you value, what you will give up, and why you still want to try your own version when a ready-made answer exists.

Those judgments will not always be right. But making the work, comparing versions, discovering a conviction worth keeping, or admitting you should change your mind—all of that is how taste develops. No Skill can go through it for you.

I want tools to save designers the repetitive work so they have the energy to give their judgment a fair chance. Try another possibility. Revisit a detail. Finally make the thing they have been carrying around in their heads.

As for this Skill that supposedly distilled generations of masters: it really does have a [SKILL.md](skills/duoasa-skill/SKILL.md). Inside is a working agreement: start from your ideas, make choices and tradeoffs clear, and help you make what you want to make. No universal master style included.

**This Skill helps the model help you be yourself.**

---

## Install and use

The actual skill lives in [skills/duoasa-skill/SKILL.md](skills/duoasa-skill/SKILL.md). Put the `duoasa-skill` folder in your client's supported skills directory. Downloading the repository alone does not activate it.

First, download the repository. These commands work in macOS, Linux, or Git Bash:

```bash
git clone https://github.com/Duoasa/Duoasa-skill.git
cd Duoasa-skill
```

Choose the commands for your client:

**Codex**

```bash
mkdir -p "$HOME/.agents/skills"
cp -R -i skills/duoasa-skill "$HOME/.agents/skills/"
```

Invoke it in a conversation:

```text
$duoasa-skill Help me develop this direction from my existing work and preferences.
```

**Claude Code (local)**

```bash
mkdir -p "$HOME/.claude/skills"
cp -R -i skills/duoasa-skill "$HOME/.claude/skills/"
```

Invoke it in a conversation:

```text
/duoasa-skill Help me develop this direction from my existing work and preferences.
```

These locations follow the [Codex documentation](https://learn.chatgpt.com/docs/build-skills) and [Claude Code documentation](https://code.claude.com/docs/en/skills). If the skill does not appear in your current session, start a new session and select it. For other Agent Skills clients, import the same folder following their instructions. In chat tools without skill support, you can read and include the file as context; that is not an installation.

The skill guides the model to work from your goals, drafts, and preferences, explain tradeoffs, help you try ideas, and reduce repetitive work. It ships no signature visual style and promises no instant taste.

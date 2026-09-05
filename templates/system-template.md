
⸻document_type: system 
name: "[Design system name]" 
id: "system.[canonical-name]" 
status: "draft" 
version: "0.1.0" 
platforms: [ios, android] 
owner: "[Design system team]" 
last_updated: "YYYY-MM-DD" 
figma_library: "[Figma library URL]" 
documentation_home: "[Documentation URL]" 
code_repositories: 
ios: "[URL]" 
android: "[URL]"


[Design system name]

System purpose

[Explain why the system exists, which products it serves, and what consistency it protects.]

Product scope

- Products: [Included products]
- Platforms: [Supported platforms]
- Users: [Primary user groups]
- Domains: [Supported domains]
- Out of scope: [Explicit exclusions]

Design principles

1. [Principle] — [Operational meaning]
2. [Principle] — [Operational meaning]
3. [Principle] — [Operational meaning]

Source-of-truth hierarchy

When sources disagree, use this order:

1. [Approved system documentation]
2. [Published Figma library]
3. [Production component library]
4. [Platform guidance]

Report conflicts rather than silently combining contradictory guidance.

## Library architecture

1. foundations/
2. components/
3. patterns/
4. templates/
5. domain-guidance/
6. content-guidance/
7. accessibility/
8. system.md


## Foundation index
Foundation	: [Name]
ID :	                Source
	    foundation.[name]	 [Status]	 [Link/path]

## Component index
Component	ID	Category	Status	Source
[Name]	component.[name]	[Category]	[Status]	[Link/path]

## Pattern index
Pattern	ID	Category	Status	Source
[Name]	pattern.[name]	[Category]	[Status]	[Link/path]

## Template index
Screen template	Purpose	Status	Source
[Name]	[Purpose]	[Status]	[Link/path]

## Global composition rules

Always

- Use documented components before creating local alternatives.
- Use semantic tokens instead of raw visual values.
- Apply a documented pattern when one matches the user task.
- Include relevant loading, empty, error, offline, and permission states.
- Preserve native platform behavior unless an approved system rule overrides it.

Never

- Invent undocumented variants, tokens, component names, or properties.
- Combine components in ways explicitly prohibited by their documentation.
- Infer missing product requirements as established design-system rules.
- Treat visual similarity as proof that two components are interchangeable.

Decision hierarchy

Use this order when composing an experience:

1. Identify the user goal and platform.
2. Select an approved pattern.
3. Select the appropriate screen template.
4. Use the documented components required by the pattern.
5. Apply semantic foundation tokens.
6. Add domain rules and product content.
7. Validate accessibility, localization, responsiveness, and system states.

Platform strategy

Shared across platforms

- [Shared principle or behavior]

iOS-specific

- [Native behavior or approved exception]

Android-specific

- [Native behavior or approved exception]

Tablet and responsive layouts

- [Adaptive-layout rule]

Accessibility baseline

- [Target standard, such as WCAG level or internal requirement]
- [Touch-target requirement]
- [Text scaling requirement]
- [Focus and screen-reader requirement]
- [Reduced-motion and non-color requirement]

Localization baseline

- Support text expansion and right-to-left layouts.
- Use locale-aware date, time, number, and currency formats.
- Do not embed text inside imagery when localization is required.
- [Additional product rule]

Content standards

- [Voice and tone]
- [Capitalization]
- [Terminology source]
- [Error-message structure]
- [Inclusive-language requirement]

Status definitions
Status	Meaning	May be used in production?
Draft	Under definition	No
Beta	Available for controlled use	With approval
Stable	Approved and supported	Yes
Deprecated	Scheduled for removal	Existing use only

Naming conventions

- IDs use lowercase dot notation: component.button.
- Filenames use lowercase kebab case: search-and-filter.md.
- Use one canonical name; record synonyms as aliases rather than duplicate entries.
- Token names describe meaning, not raw appearance.

AI usage instructions

When using this system to generate or evaluate designs:

1. Retrieve this file first.
2. Retrieve the relevant pattern before selecting components.
3. Retrieve every referenced component and foundation file.
4. Follow always, never, and composition constraints literally.
5. Distinguish documented facts from recommendations and assumptions.
6. List missing requirements instead of inventing system guidance.
7. Cite the IDs of the rules and assets used in the result.

Contribution and governance

- Propose: [Who may propose changes]
- Review: [Required reviewers]
- Approve: [Approval owner]
- Publish: [Publishing responsibility]
- Deprecate: [Deprecation process]

Release and versioning

- Versioning model: [Semantic or internal versioning]
- Release cadence: [Cadence]
- Change log: [Location]
- Migration guidance: [Location]

Known gaps

- [Missing component, pattern, platform, or implementation]

Change history
Version	Date	Change	Owner
0.1.0	YYYY-MM-DD	Initial draft	[Owner]

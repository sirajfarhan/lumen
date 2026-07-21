# Web Style Stack

Use this reference when the site needs strong art direction. Also use it for a greenfield build with no design system and for a generated page that looks competent but generic.

## Core Rule

Style is proof. It is the visible body of the story model. The visual system should make the visitor believe they entered the right world for the claim. Choose tools because they reduce the distance between the intended world and a rendered site that is accessible enough to inspect honestly.

Treat frameworks as primitives that serve art direction. Tailwind gives a fast token and layout language. shadcn/ui gives editable component code. Radix, Base UI, and React Aria give accessible primitives. Motion and GSAP give time. React Three Fiber and Drei give spatial embodiment. The art direction still has to come from the visitor change and the proof substrate inside the chosen carrier.

## Default Stack Shape

For greenfield React work, Vite is usually the fastest local build surface. Move to another framework when the user needs server routing, SEO architecture, or an existing repo already points elsewhere. Keep React as the execution world unless the existing project or user asks for another stack.

Use Tailwind CSS as the default high-control styling layer when the project convention allows it. Its value is fast control over spacing that stays tied to type and color. It also keeps responsive behavior and state close to the token system. In Tailwind v4, theme variables and CSS-first configuration make it especially useful for custom visual worlds.

Use shadcn/ui when the site needs polished accessible components that can be owned and restyled as local code. Use Radix UI or Base UI when the design needs deeper custom primitives with full custom visual control. Use React Aria Components when interaction complexity and accessibility behavior are central enough to justify the extra model.

Use Motion for React as the ordinary animation layer. It fits small interface state changes and modest story rhythm. Use GSAP when the site needs a choreographed timeline, scroll-synced sequence, or precise animation control that earns a stronger result than Motion.

Use React Three Fiber with Drei when the 3D gate passes. React Three Fiber lets the spatial proof stay inside React. Drei earns its place when helper components reduce fragile Three.js setup. A 3D stack is ready when it makes the spatial relation easier to reconstruct and gives spectacle a proof job.

Use a specialized visual library when its medium is the proof. A site that needs one honest comparison may be served by a small SVG or CSS chart. A site that needs a real spatial scene may need Three.js. Choose the lightest tool that lets the visitor reconstruct the story.

## Carrier To Stack

A reading surface usually needs typography to carry composition while imagery gives the section rhythm a body. Start with Tailwind tokens and custom CSS where needed. Use a component library only when real behavior needs an accessible primitive.

A guided story surface needs pacing. Use Motion for section reveal or state continuity when the timing makes the sequence easier to follow. Let scroll behavior earn its place by making the sequence clearer than layout alone.

An evidence surface needs trust. Put the source close enough that a claim can be checked where it appears. Use a chart library when the visitor needs inspection, comparison, or filtering. Keep style quiet enough that the evidence remains the object.

A product surface needs clear action and credibility. Use shadcn/ui when local component ownership matters. Use Radix, Base UI, or React Aria when controls need deeper accessibility behavior. The page should feel authored for this product through its own components and states.

A story-tool needs state behavior. Component primitives should make the form state and keyboard path feel natural. Writer-shaped labels and empty states matter here because the visitor touches the story through words.

A spatial world needs embodied relation. Use 3D only after the spatial gate passes. Keep a flat fallback and visible landmarks so reset, reduced motion, and mobile framing remain humane. The scene must explain the site through the physical relation that matters.

## Style Proof Pass

Before implementation, write one sentence for the visual target. It should name the world under visitor pressure and the proof material that makes that world believable. Make it specific enough that it clearly belongs to this site.

Choose tokens before components. Name how type creates density and how color creates state. Name how surfaces behave before choosing primitives. Let component kits inherit the chosen visual texture through an intentional token system.

Use visual references as calibration. Borrow the invariant and transform the surface. One reference might teach restraint. Another might teach how sequence earns trust through space or time. A code-bearing reference might teach a reusable mechanism. The generated site should feel new.

During screenshot inspection, ask five questions together. What world did I enter? What proof material is visible? Which framework choice made the result better or faster? Which element still needs a more specific visual job? What would break if this style were swapped onto another site?

When the answer is mostly “nice page,” return style to the visitor proof. When generated sites look similar, make the token system and carrier-to-stack choice more specific. When the site is beautiful and the visitor needs a clearer purpose, repair the story route. When the site is clear and flat, add the style detail that increases correct reconstruction for less effort.

When a source shaped the build, run a source-transfer review after the site renders. Treat it as a craft comparison, not a likeness contest. Ask whether the chosen source solved the same pressure. Then ask whether the useful mechanism survived. Then ask whether the result moved far enough from source identity. Craft should stay comparable at the new scale. The medium should make understanding stronger. A viewer should see the user's site as its own world. The lowest gate controls repair.

Score with restraint. Prototype success belongs mostly in the sixties, seventies, and low eighties until direct rendered inspection proves stronger craft. A ninety means the current artifact has survived source-aware comparison, cold reconstruction, and mobile inspection with only small local repairs left. One hundred is the horizon the work moves toward.

For 2D inspiration, compare the reading path first. The page should lead attention through the borrowed move. Proof should sit where the claim needs it. The same relation should survive at narrow width. Component state should clarify the move when interaction carries it. The strongest 2D source transfer can look visually distant from the source while preserving the hierarchy that carries proof. It should preserve rhythm. It should keep proof close to the claim. It should preserve the state logic.

For 3D inspiration, compare the spatial operation first. Camera work should turn scale with depth and occlusion into one readable law. Landmarks should make orientation recoverable. Reset and fallback should keep burden humane. Input should feel like understanding. 3D earns selection when depth creates clearer reconstruction than the best flat alternative. A 3D result needs more evidence than a 2D result because the rendered scene can look impressive while the visitor loses the story. Score camera framing first. Then score scale and depth. Then score occlusion. Then score landmark clarity. Then score input burden. Then score mobile canvas framing and flat-fallback gain before raising quality parity.

Use production-craft scoring as a separate pressure when the user wants exceptional visual quality. Acceptance begins when every source-transfer gate clears the floor. Production craft begins when `quality_parity` also clears the chosen target and direct screenshots show a fully authored surface. Type should fit. Canvas space should carry a story job. Component residue should be transformed. Material worlds should match. Interaction should feel authored rather than borrowed.

## Reference-Led Build

When a run needs award-level or highly artistic quality, the stack decision should be preceded by source contact. Search visually first to calibrate taste. Then search implementation sources that a developer could actually inspect. A gallery can show the target level of attention, but a public demo or repository can show how a mechanism is built. Keep those two uses separate.

Use source candidates by carrier. A reading surface learns from editorial rhythm. A guided story surface learns from pacing. An evidence surface learns from proof placement. A product surface learns from component behavior. A story-tool learns from state. A spatial world learns from orientation and burden control.

Code adaptation should start from sources that are meant to be reused. Official examples are safer than copied sites. Component registries are useful when the page needs owned React pieces. Public demos and licensed repositories are useful when the mechanism is visible. shadcn/ui blocks and compatible local component code are strong for owned React surfaces. Motion examples can guide small interface transitions. GSAP demos can guide timeline structure when choreography is the proof. React Three Fiber and Drei examples can guide spatial mechanics after the 3D gate passes. Community projects on GitHub can help when they match the carrier, but inspect license and source shape before borrowing.

Separate setup contact from mechanism contact. Setup contact explains how the local app runs. Mechanism contact explains how the hard part of the site should work. A Vite guide can support the run. A React starter can support it too. Package docs can help the shell. Generic layout references can help baseline behavior. Generated visuals and earlier local artifacts can help the evidence record. For a high-ambition build, the mechanism source should reveal the move being adapted through a reusable example or inspectable project source.

Use the carrier to choose the mechanism search. A reading surface looks for editorial rhythm only when that rhythm changes reading. A guided story surface inspects scroll or reveal mechanics when pacing is part of the proof. An evidence surface inspects the charting or annotation pattern that keeps proof near claim. A product surface inspects component ownership and action states. A story-tool inspects the control pattern that makes state legible. A spatial world inspects camera behavior first. It then checks landmarks, fallback behavior, and performance risk. The borrowed mechanism should be small enough to transform and strong enough to improve the build.

Use award sites and proprietary pages to extract visual law while transforming surface identity. That law may live in density. It may live in pacing. It may live in material contrast. It may live in navigation relation. It may live in proof placement or interaction expectation. The implementation should be transformed through the user's content. It should also transform the route decision. The token system, responsive law, and component architecture should become native to the user's site.

The efficient path is small but real. Open the source. Inspect the files or docs that carry the useful move. Decide whether it is code, pattern, or inspiration only. Record the borrowed invariant and the legal boundary. Then build the smallest transformed React version that proves the move in the user's site.

## Current Source Panel

These sources justify the default stack shape. Re-check them when a user asks for the latest best stack or when a project has unusual constraints. The current source panel uses official documentation for the styling layer. It also covers accessible primitives. It covers animation. It covers spatial React work and the local React build path.

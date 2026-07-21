# Writer Tone Of Voice Template

## Purpose

Writer voice is user-specific. The exported skill includes this blank template so each user or organization can build its own voice reference without shipping another person's style profile inside the plugin.

Use this reference when Writer needs to shape reader-facing material and no current voice profile is available for the active user, organization, or project.

## Voice Readiness Route

Start from the least burdensome evidence source available. The goal is to clear Voice Readiness with enough direct evidence to protect the current surface, not to complete a long interview.

1. Resolve scope: user, organization, or project.
2. Preview Writer memory and reuse an active profile only when it belongs to the active scope and writing surface.
3. If the user provides past writing samples, extract a draft voice profile from the closest matching samples.
4. If samples are missing, ask one small contrast question that changes the next draft.
5. If one answer can reveal the missing boundary faster, offer two short calibration fragments and ask which feels closer, plus the smallest reason why. These are calibration fragments, not final drafts.
6. If the user corrects a draft, treat the correction as the strongest current evidence. Record whether it changed wording, audience calibration, concept order, causal story, or the intended outcome.
7. If memory is available, capture durable learning as Writer skill memory. If memory is local-only, keep the filled profile local until sync is available.

Do not require a full interview. Submit the current voice evidence to Lumen and ask only its returned next question while the track is calibrating. Do not draft the requested final surface until Lumen returns an executable proof.

## Evidence Modes

```text
reuse               existing scoped profile matches this user, org, project, and writing surface
sample_digest       user supplied prior writing or a known approved artifact
one_contrast        one answer can change the next draft
pairwise_calibrate  two short variants can reveal the better direction faster than more explanation
correction_loop     user edits or rejects a real draft
```

Escalate only when the current evidence cannot guide the next draft. Stop when another question would preserve the same draft direction.

## Blank Profile

```yaml
profile_owner:
  user_id:
  organization_id:
  project_id:
  scope: user | organization | project

voice_state:
  status: draft | active | needs_review
  confidence: low | medium | high
  readiness_state: unknown | calibrating | executable | enriching | verified | transfer_confirmed | invalidated
  readiness_evaluation_id:
  evidence_mode:
  memory_decision:
  invalidation_trigger:
  writing_surface:
  evidence_mode: reuse | sample_digest | one_contrast | pairwise_calibrate | correction_loop
  source_evidence:
    - label:
      kind: sample | correction | stated_preference | observed_pattern
      public_summary:
      hash:

preferred_movement:
  reader_effect:
  emotional_temperature:
  density:
  directness:
  rhythm:

reasoning_movement:
  shared_context_entry:
  outcome_frame:
  problem_before_solution:
  concept_introduction:
  example_role:
  action_landing:

audience_adaptation:
  knowledge_baseline:
  concepts_to_explain:
  labels_to_delay_or_omit:
  preferred_technical_depth:

concept_language:
  verbs_that_name_the_real_action:
    -
  broad_words_to_soften_when_needed:
    -
  concrete_replacements:
    -

language_patterns:
  usually_preserve:
    - 
  usually_avoid:
    - 
  tolerated_when:
    - 

correction_memory:
  rejected_patterns:
    -
  accepted_patterns:
    -
  premise_change_triggers:
    -
  why_the_accepted_movement_worked:
  evidence_status: confirmed | provisional
  scope_for_reuse: user | organization | project | relationship | surface
  superseded_by:

fit_check:
  how_the_current_draft_matches:
  where_it_may_drift:
  repair_if_it_drifts:
  profile_update_decision: keep | update | ask_one_contrast | ask_pairwise_choice
```

## Validation Evidence

For a Writer validation packet, include a public voice handle:

```text
voice profile summary
voice readiness proof
voice evidence tier or mode
voice source evidence or hash
voice fit notes for the current final draft
drift risk
profile update decision
```

The packet should make the voice target inspectable without exposing private examples unnecessarily. Use a hash or short public summary when raw samples are sensitive.

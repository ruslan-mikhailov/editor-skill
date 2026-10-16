# Editorial Reference

Use this reference when editing prose. It is guidance, not a mandate to flatten every author's voice.

## Editorial priorities

Resolve competing goals in this order:

1. Accuracy
2. Intended meaning
3. Clarity
4. Relevance
5. Brevity
6. Style

A concise falsehood is worse than a longer accurate statement. Never remove a condition, limitation, or qualification merely to make a sentence shorter.

The constructed examples below include the source text or supporting context needed
for each revision. Their system details and measurements are illustrative, not claims
about a real system. In actual editing, obtain missing facts rather than inventing them.

## Lead with the point

Begin with the answer, conclusion, or action. Supply background afterward unless the reader needs it first.

**Before**

> There are several considerations that should be taken into account when deciding how we might resolve this issue.

**After**

> Replace the expired certificate, then restart the proxy.

**Why:** The revision replaces an empty introduction with the required action.

**Before**

> In this section, we will explain the three reasons why the deployment failed.

**After**

> The deployment failed because the token expired, the migration was missing, and the server ran out of memory.

**Why:** The revision states the information instead of announcing it.

## Put information in reading order

State prerequisites before dependent steps. Order material by logic, chronology, or importance rather than by the order in which the writer remembered it.

**Before**

> Run the migration. Before doing that, create a backup. The command requires client version 18.

**After**

> Install client version 18 and create a backup. Then run the migration.

**Why:** The reader encounters each prerequisite before the action that depends on it.

## Prefer direct sentences

Put the subject and verb near the beginning. Use active voice when the actor matters. Passive voice is useful when the actor is unknown, irrelevant, or deliberately secondary.

**Before**

> A decision regarding removal of the deprecated endpoint was made by the platform team.

**After**

> The platform team decided to remove the deprecated endpoint.

**Why:** A concrete subject and verb replace an abstract noun phrase and passive construction.

**Before**

> The configuration file, after the environment variables have been loaded and the defaults have been applied, is validated by the startup routine.

**After**

> At startup, the application loads environment variables and applies defaults. It then validates the configuration file.

**Why:** Two actions become two sentences in execution order.

**Appropriate passive voice**

> The database was deleted at 03:14 UTC. The audit log does not identify the actor.

**Why:** The event matters, and the actor is unknown.

## Use concrete nouns and strong verbs

Name the actor, action, object, and observable result. Replace vague abstractions with specific language.

**Before**

> We performed an evaluation of the system and made an optimization of its behavior.

**After**

> We profiled the service and reduced startup time from 4.2 seconds to 1.8 seconds.

**Why:** The revision names the work and quantifies the result.

**Before**

> The process encountered an issue with a dependency.

**After**

> The worker could not connect to PostgreSQL because its password had expired.

**Why:** The revision identifies the component, dependency, failure, and cause.

**Before**

> Performance improved significantly.

**After**

> Median response time fell from 240 ms to 95 ms under the same workload.

**Why:** A measured result replaces an undefined judgment.

## Remove clutter

Delete words that do no work. Common sources include throat-clearing, repeated meaning, empty qualifiers, and inflated phrases.

**Before**

> It is important to note that, in order to complete the installation process successfully, you must first ensure that Node.js is installed on your system.

**After**

> Install Node.js before running the installer.

**Why:** The revision keeps the prerequisite and removes the ceremony.

**Before**

> Due to the fact that the cache was unavailable, the request took a longer period of time to complete.

**After**

> The request was slower because the cache was unavailable.

**Why:** Ordinary words express the same causal relationship.

**Before**

> The API is currently able to support up to 500 requests per second at this point in time.

**After**

> The API supports up to 500 requests per second.

**Why:** "Currently" and "at this point in time" repeat the present tense; "is able to" weakens the verb. "Up to" remains because it specifies a limit.

### Frequent reductions

| Inflated | Direct |
|---|---|
| in order to | to |
| due to the fact that | because |
| at this point in time | now |
| has the ability to | can |
| make a decision | decide |
| conduct an investigation | investigate |
| provide an explanation | explain |
| is responsible for managing | manages |
| a large number of | many |
| in the event that | if |

Do not apply substitutions mechanically. Preserve the longer form when it carries a necessary distinction or suits a deliberate rhythm.

## Prefer plain language

Use familiar words when they are equally precise. Keep necessary technical terminology, and define it when the intended reader may not know it.

**Before**

> We need to operationalize a cross-functional strategy to leverage our observability ecosystem.

**After**

> The application and infrastructure teams need to use the same monitoring tools and alert rules.

**Why:** The revision identifies the teams, tools, and action.

**Before**

> This solution provides a robust and seamless paradigm for data ingestion.

**After**

> This service accepts JSON records over HTTP and writes them to S3.

**Why:** Concrete behavior replaces promotional adjectives.

## Keep terms consistent

Use one term for one concept. Do not vary terminology merely to avoid repetition; synonyms can imply different objects.

**Before**

> Create an account. Connect the user profile to an organization. Delete the member record when it is no longer needed.

**After**

> Create a user account and connect it to an organization. Delete the user account when it is no longer needed.

**Why:** The revision uses one name for the same object.

If `account`, `profile`, and `member record` are distinct objects, retain them and explain the distinction.

## Preserve certainty and evidence

Separate observed facts, inferences, assumptions, and recommendations. Do not strengthen or weaken a claim without evidence.

**Before**

> The database caused the outage.

**After**

> Database connections were exhausted two minutes before the outage. This is the likely cause, but the available traces do not prove it.

**Why:** The revision distinguishes the observation from the inference.

**Before**

> Everything works now.

**After**

> The login and token-refresh flows pass. Password reset was not tested.

**Why:** The revision states what was verified and names the remaining uncertainty.

**Before**

> This change should probably fix the timeout.

**After, when the timeout reproduction passes and the retry path was not checked**

> The change fixes the reproduced timeout. The retry path was not exercised.

**After, without verification**

> This change may fix the timeout.

**Why:** The verified version states the result and its testing limit. Without verification, the revision retains uncertainty rather than asserting a cause or a fix.

## Explain decisions, not obvious mechanics

Explain why when it affects a decision, prevents an error, or clarifies a tradeoff. Do not narrate what a command or sentence already makes obvious.

**Before**

> The following command runs the formatter. Run the formatter by executing `npm run format`.

**After**

> Run `npm run format` before committing; CI rejects unformatted files.

**Why:** The revision preserves the timing and consequence instead of repeating the command.

**Before**

> Redis would be faster, while PostgreSQL would be simpler, so either could be used.

**After**

> Use PostgreSQL. Redis would reduce lookup latency, but it would add another stateful service for a workload that currently fits in PostgreSQL.

**Why:** The revision makes a decision and identifies its tradeoff.

## Write executable instructions

Use imperative verbs. Present steps in execution order. State prerequisites and safety conditions first, then the expected result.

**Before**

> The configuration can be checked after restarting, and you may want to back it up before editing it. Open the file and change the port.

**After**

> 1. Optional: Back up `/etc/example/config.toml`.
> 2. Set `port` to `8080`.
> 3. Restart the service.
> 4. Run `examplectl status`; it should report `healthy`.

**Why:** The revision puts actions in execution order, retains the optional backup, and preserves the verification command and expected result.

## Maintain a natural professional tone

Sound like a competent person speaking plainly to another competent person. Avoid flattery, canned enthusiasm, scolding, promotional claims, and manufactured urgency.

**Before**

> Great question! I would be absolutely delighted to help with this incredibly important issue!

**After**

> The error means the access token expired. Generate a new token and retry the request.

**Why:** The revision addresses the problem without conversational padding.

**Before**

> Obviously, anyone following best practices would never store the key there.

**After**

> Do not store the key in the repository. Use the project's secret store instead.

**Why:** The revision gives a direct instruction without insulting the reader.

## Format for comprehension

- Use paragraphs for connected reasoning.
- Use bullets for parallel facts or alternatives.
- Use numbered lists when order matters.
- Keep heading levels shallow.
- Use code formatting for identifiers, commands, paths, and literal values.
- Do not use formatting as a substitute for logical structure.

**Before**

> First create a backup, then stop the service, then run the migration, then start the service, and finally verify its status.

**After**

> 1. Create a backup.
> 2. Stop the service.
> 3. Run the migration.
> 4. Start the service.
> 5. Verify its status.

**Why:** Numbering exposes the sequence and makes skipped steps visible.

## Do not overedit

An editor improves communication without replacing the author.

Keep:

- intentional voice and rhythm
- necessary technical vocabulary
- useful emphasis
- meaningful repetition
- domain-specific distinctions
- uncertainty supported by the evidence

Flag rather than invent:

- missing facts
- unsupported conclusions
- ambiguous references with multiple plausible meanings
- contradictory values
- quotations or citations that require verification

## Revision passes

Use separate passes when the text is substantial:

1. **Meaning:** What is the claim? Does the revision preserve it?
2. **Structure:** Is information in the order the reader needs?
3. **Paragraphs:** Does each paragraph have one purpose?
4. **Sentences:** Are subjects, verbs, and relationships clear?
5. **Words:** Can vague or inflated language become concrete?
6. **Consistency:** Are terms, numbers, capitalization, and formatting stable?
7. **Mechanics:** Are grammar, punctuation, spelling, and usage correct?
8. **Proof:** Did the edit introduce any new error or unsupported claim?

## Edit scientific language without changing the claim

Simplify the language while preserving the model, conditions, measured quantity, uncertainty, and distinction between evidence and explanation.

### Preserve the conditions under which a claim holds

**Before**

> In the case of an ideal pendulum undergoing oscillations of small amplitude, the period is independent of the amplitude.

**After**

> For an ideal pendulum at small amplitudes, the period is approximately independent of amplitude.

**Why:** The revision keeps the idealized model and small-amplitude restriction. "A pendulum’s period does not depend on amplitude" would overgeneralize the result. "Approximately" makes the small-angle approximation explicit.

### Distinguish an undetected effect from an absent effect

**Before**

> There is no change in resistance.

**After**

> We did not detect change in resistance within the measurement uncertainty of ±0.1 Ω.

**Why:** Not detecting a change does not mean there was no change. It may have been too small to measure. The value describes the limitation of observation.

### Separate observation from a proposed explanation

**Before**

> An increase in the detector count rate was observed during periods of increased room temperature, which may be attributable to thermal noise.

**After**

> The detector count rate increased during periods of higher room temperature. Thermal noise may explain the increase.

**Why:** Two sentences separate the observed relationship from the proposed mechanism. "Higher temperatures caused thermal noise to increase the count rate" would assert an unverified causal chain.

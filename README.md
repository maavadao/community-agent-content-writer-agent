# Content Writer Agent

Turns an approved outline into a first draft: article, video script, lesson text or social post, in the creator's voice.

Stage 2 of 3 in the content lifecycle (research and plan → create → review and publish).

Takes an outline and sources (from the Content Research Agent or the creator's own) and writes a draft at the right reading level. It keeps the creator's wording where they supply it, adds a citation for every factual claim, and flags places where the creator should add their own experience.

## Run it

Needs a running [maava gateway](https://github.com/maavadao/maava-gateway) with its chat endpoint
enabled. See the [getting started guide](https://github.com/maavadao/maava-Community-Agents/blob/main/docs/getting-started.md).

```bash
pip install -r requirements.txt
cp .env.example .env   # then set MAAVA_GATEWAY_TOKEN
export $(grep -v '^#' .env | xargs)
python src/main.py "your request"
```

Its brief is in [`instructions.md`](instructions.md).

## Data

Content you provide is processed to answer you and is not kept after the session. No accounts or analytics.

## Part of maava Community Agents

This agent is one of the [maava Community Agents](https://github.com/maavadao/maava-Community-Agents),
listed on [maavadao.com/agents](https://maavadao.com/agents). Read the
[rules](https://github.com/maavadao/maava-Community-Agents/blob/main/RULES.md) and
[contributing guide](https://github.com/maavadao/maava-Community-Agents/blob/main/CONTRIBUTING.md)
before you open a pull request. When the agent earns money, 60% rewards the developer community
who built it and 40% goes to Maava Charity to educate children in need.

## Licence

Apache 2.0.

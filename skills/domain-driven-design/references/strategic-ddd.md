# Strategic DDD

Strategic DDD decides where models live and which parts of the domain deserve
focus.

## Subdomain Types

- Core domain: differentiating business capability. Invest in deep modeling.
- Supporting domain: important but not differentiating. Model enough to support
  core flow.
- Generic domain: common capability. Prefer standard product or commodity
  solution when possible.

## Checks

- What creates business advantage?
- Which subdomain changes most often?
- Which subdomain needs domain expert attention?
- Which parts can be bought or reused?
- Which context owns which language?

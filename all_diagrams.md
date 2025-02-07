 # Mermaid diagrams

 Creating this file to check how github behaves with Mermaid and what VS Code plugins might be useful.

 All examples adopted from Mermaid official docs and examples - [here](https://docs.mermaidchart.com/mermaid/intro)

 ## Flowchat

 A very basic exampe below. Lots of edges and shapes are available.

 ```mermaid
 graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

```mermaid
flowchart LR
      A[Start]-->B[Do you have coffee beans?]
      B-->|Yes|C[Grind the coffee beans]
      B-->|No|D[Buy ground coffee beans]
      C-->E[Add coffee grounds to filter]
      D-->E
      E-->F[Add hot water to filter]
      F-->G[Enjoy!]
```

## Sequence diagrams

Probably the most important type of diagram for visualizing the various flows.

```mermaid
 sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```
## Gitgraph

This could be used to visalize how we work with branches etc. in the CAMARA project and/or DN specific WoW (if any)


```mermaid
 gitGraph
       commit
       commit
       branch develop
       commit
       commit
       commit
       checkout main
       commit
       commit

```

## Mindmap

This is my favourite diagram type for maintaining backlog / list of ideas, etc. Very lightweight and visual.

```mermaid
mindmap
      root((mindmap))
        Origins
          Long history
          ::icon(fa fa-book)
          Popularisation
            British popular psychology author Tony Buzan
        Research
          On effectiveness <br/> and features
          On Automatic creation
            Uses
                Creative techniques
                Strategic planning
                Argument mapping
        Tools
          Pen and paper
          Mermaid
```

## Quadrant

```mermaid
quadrantChart
    title Reach and engagement of campaigns
    x-axis Low Reach --> High Reach
    y-axis Low Engagement --> High Engagement
    quadrant-1 We should expand
    quadrant-2 Need to promote
    quadrant-3 Re-evaluate
    quadrant-4 May be improved
    Campaign A: [0.3, 0.6]
    Campaign B: [0.45, 0.23]
    Campaign C: [0.57, 0.69]
    Campaign D: [0.78, 0.34]
    Campaign E: [0.40, 0.34]
    Campaign F: [0.35, 0.78]
```

## More examples

* [Link1](https://docs.esa.io/posts/308)
# GDRB
Graph Data Regularities Benchmark (GDRB)

## Preliminary work.

Fact Checking Benchmarks (unpublished draft).pdf

## GFC documents

Paper: 2018-DASFAA-GFC-paper.pdf

Slides: 2018-DASFAA-GFC-slides.pptx

Source Code: SourceCode-GFC/

## Reference

```
@inproceedings{lin2018discovering,
  title={Discovering Graph Patterns for Fact Checking in Knowledge Graphs},
  author={Lin, Peng and Song, Qi and Shen, Jialiang and Wu, Yinghui},
  booktitle={International Conference on Database Systems for Advanced Applications},
  pages={783--801},
  year={2018},
  organization={Springer}
}
```

## Quick build and test

### Requirements

JDK 1.8+ and Maven 3.0+

### GFC (Graph Fact Checking Rules)
```java
$ mvn package
$ java -cp ./target/factchecking-1.0-SNAPSHOT-jar-with-dependencies.jar \
        edu.wsu.eecs.gfc.exps.TestGFC \
		./sample_data/ \
		./output \
		0.01 \
		0.0001 \
		4 \
		50
```

### OGFC (Graph Fact Checking Rules with Ontology Closeness Enabled)

```java
$ mvn package
$ java -cp ./target/factchecking-1.0-SNAPSHOT-jar-with-dependencies.jar \
        edu.wsu.eecs.gfc.exps.TestOGFC \
		./sample_data/ \
		./output \
		0.01 \
		0.0001 \
		4 \
		50
```

### Contact

peng.lin@wsu.edu

http://eecs.wsu.edu/~plin1

### License

MIT License

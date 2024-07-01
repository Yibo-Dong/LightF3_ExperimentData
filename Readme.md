# Experiment Data

## Introduction

The data for our experiments is organized here.

## File Organization

```
|─ License
|─ Readme.md
|─ bcar								// verifier
|─ fcar
	|── fcar-Alice						// Verifier-Station
		|──  Alice-00001.log				// CAR log
		└──  Alice-00001.res				// CAR result
|─ ic3-ref 
	|── ic3-ref-Alice						  
		└──res						// IC3-ref result
|─ iimc-bmc
|─ iimc-ic3
	|── iimc-ic3-Alice						
		|── Alice-00001					// iimc-ic3
		|── ...
```

## Configuration

### Command Line Option

| Verifier     | Command Line Option |
| ------------ | ------------------- |
| Forward CAR  | -f                  |
| Backward CAR | -b                  |
| IC3-ref      | -s                  |
| IIMC-ic3     | -t ic3              |
| IIMC-bmc     | -t bmc              |

### Station Size

| station | Track | Route | Switch | Signal |
| ------- | ----- | ----- | ------ | ------ |
| Alice   | 14    | 8     | 3      | 12     |
| Bob     | 56    | 70    | 14     | 37     |
| Charlie | 171   | 503   | 87     | 152    |
| David   | 151   | 720   | 79     | 145    |
| Eve     | 151   | 499   | 74     | 140    |



## Time Consumption

###   Instantiation Time Consumption

| station | Time(s) |
| ------- | ------- |
| Alice   | 5       |
| Bob     | 14      |
| Charlie | 731     |
| David   | 858     |
| Eve     | 855     |

###   Aiger Generatation Time Consumption

| station | Time(s) |
| ------- | ------- |
| Alice   | 28      |
| Bob     | 142     |
| Charlie | 1195    |
| David   | 1369    |
| Eve     | 1422    |

###     Verification Time Consumption

| station | BCAR(s) | FCAR(s) | IC3-ref(s) | IIMC-ic3(s) | IIMC-bmc(s) |
| ------- | ------- | ------- | ---------- | ----------- | ----------- |
| Alice   | 4       | 25205   | 33         | 833         | 11639       |
| Bob     | 118     | 43939   | 1201       | 60966       | 51772       |
| Charlie | 1610    | 31629   | 18541      | 53589       | 44199       |
| David   | 1424    | 23519   | 12768      | 39963       | 29475       |
| Eve     | 15982   | 65390   | 35397      | 114600      | 79831       |

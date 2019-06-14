## Requirements
python >= 3.6
pytorch == 0.3.0
## Dataset
|BC|PB|ZX
--|:--:|:--:|--:
train | 52,433|5,140|1,649
dev | 998 |1,300 |500
test |1,995 |2,600 | 1,100
unlabeled | - | 326,981 |32,492

## Performance
  Final results on the test data:
  PB| | |ZX
  | UAS | LAS |UAS |LAS
  Trained on single-domain data
BC-train |67.55|61.01|**68.44**|59.55
PB-train |**74.52**|**69.02**|51.62|40.36
ZX-train |52.24|42.76|68.14|**61.71**
  Trained on source- andtarget-domain data
  MTL | 75.39 |69.69|72.11|65.66
  concat | 77.49 | 72.16 |76.80 |70.85
  DOEMB | 78.24|72.81|77.96|72.01
  +ELMo |77.62|72.35|78.50|72.49
  +Fine-tuning | **82.05** |**77.216**|**80.44**|**75.11**
## Usage



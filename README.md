# my-ecg-detector-test-data
the test data for my c++ ecg rpeaks detecter project:https://github.com/chaos0607/ecg_detector



originally data form: https://github.com/berndporr/ECG-GUDB/tree/master/docs/experiment_data



i applied my ECG detector and save my R-peak results in rpeaks_twoaverage.tsv and rpeaks_wqrs.tsv.

use a modified script jf_stats_detectors.py from https://github.com/berndporr/JF-ECG-Benchmark to check the score of the detector



**2024/07/29** 

​	current data is correspond to  ecg_detector version0.1

​	this is the score for  c++ ecg rpeaks detecter

![](analysis_results/cpp_cs_v0.1.png)

original result data:

`<!--**JF Score: sitting chest strap**-->`
`<!--**two_average_detector: 98.9+/-5.6**-->`
`<!--**wqrs_detector: 90.2+/-16.0**-->`

`<!--**JF Score: maths chest strap**-->`
`<!--**two_average_detector: 97.1+/-10.2**-->`
`<!--**wqrs_detector: 91.7+/-18.2**-->`

`<!--**JF Score: walking chest strap**-->`
`<!--**two_average_detector: 97.7+/-7.8**-->`
`<!--**wqrs_detector: 89.9+/-18.3**-->`

`<!--**JF Score: hand bike chest strap**-->`
`<!--**two_average_detector: 93.7+/-12.0**-->`
`<!--**wqrs_detector: 83.9+/-19.9**-->`

`<!--**JF Score: jogging chest strap**-->`
`<!--**two_average_detector: 86.9+/-14.6**-->`
`<!--**wqrs_detector: 74.5+/-17.6**-->`



​	this the score for the originally python ecg rpeaks detecter

![](analysis_results/python_cs.png)



original result data:

`JF Score: sitting chest strap`
`two_average_detector: 97.7+/-7.8`
`wqrs_detector: 90.2+/-16.0`

`JF Score: maths chest strap`
`two_average_detector: 91.4+/-14.2`
`wqrs_detector: 91.7+/-18.2`

`JF Score: walking chest strap`
`two_average_detector: 93.6+/-11.6`
`wqrs_detector: 89.9+/-18.3`

`JF Score: hand bike chest strap`
`two_average_detector: 91.3+/-13.1`
`wqrs_detector: 83.9+/-19.9`

`JF Score: jogging chest strap`
`two_average_detector: 84.1+/-23.5`
`wqrs_detector: 74.5+/-17.6`



​	from this two groups results, we can see that the result of cpp detectors matched the precision of original python detectors, however , both of them have bad performance on wqrs detection. which needs future work 


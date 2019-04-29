# continous delivery for machine learning
### overview

Short summary (derived from https://emilygorcenski.com/post/data-versioning/)
- what makes cd4ml hard is that we have a lot of things that can and will change
- subject to change:
  - the training code (hyperparameters & code, should be versioned)
  - the trained model (final artifact, usually a compiled file format, should be versioned)
  - the training data preperation pipeline (code, should be versioned)
  - the raw data fed into the beginning of the pipeline (not necessarily versioned, but the output of this pipeline has to be versioned)
  - the schemas of data at each processing step (should ideally be versioned)
- existing approaches
  - models (algorithmic approach + hyperparameters) as code (simplifies versioning, but stronger coupling)
  - version control for data (e.g. by hashing blob datasets) used in the tools MLFlow, Pachyderm, and dvc. Helps with reproducable builds and sharing work. Downsides are immature tooling and huge storage demands.
  
Relevant technologies

CI4ML platforms
- https://dvc.org
- https://www.pachyderm.io
- https://www.tensorflow.org/tfx

 formats
- https://onnx.ai/ interchangable ml format
- http://avro.apache.org

pipelines as code

- https://airflow.apache.org
- https://concourse-ci.org/
- https://github.com/kubeflow/kubeflow

tutorials / workshops
- https://github.com/ThoughtWorksInc/continuous-intelligence-workshop
- https://www.tensorflow.org/tfx/tutorials/tfx/workshop

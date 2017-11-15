# week1-day4-tensorboard

Practice guide & note for Students.

Part of [AIRI-400](http://airi.kr/airi400/curriculum/) program.

Week1, Day4, Afternoon (2017.9.7)


# WEEK1_DAY4_Tensorboard_Summary_Note

- `tf.summary.FileWriter(dir_path,graph)`
- `tf.summary.scalar(a_tensor)`
- `writer.add_summary()`


# WEEK1_DAY4_Tensorboard_Embedding_Note

- `from tensorflow.contrib.tensorboard.plugins import projector`
- `config = projector.ProjectorConfig()`
- `embedding = config.embeddings.add()`
- `embedding.metadata_path = 'metadata.tsv'`
- `embedding.sprite.image_path = 'sprite.png'`
- `embedding.sprite.single_image_dim.extend([28, 28])`
- `projector.visualize_embeddings(writer, config)`


# WEEK1_DAY5_Tensorflow_Tips_Note

- `config.gpu_options.allow_growth = True`
- `CUDA_VISIBLE_DEVICES`
- `tf.train.Saver()`
- `tf.train.export_meta_graph()`
- `tf.train.import_meta_graph()`
- `inspect_checkpoint.py`
- `tf.get_default_graph().finalize()`
- `tf.reset_default_graph()`
- `tf.check_numerics(tensor,messge)`
- `python -m pdb myscript.py`
- `from tensorflow.python import debug as tf_debug`
- `sess = tf_debug.LocalCLIDebugWrapperSession(sess)`


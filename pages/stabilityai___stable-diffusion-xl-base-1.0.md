-
- ```
  pose_list = [
      "downward dog pose, studio background",
      "warrior II pose, studio background",
      "tree pose, studio background"
  ]
  instructions = [
      "Let's start with a gentle downward dog. Keep your back straight and breathe deeply.",
      "Now move to warrior two pose, arms stretched out, feel your legs strong.",
      "Finally, tree pose. Balance on one leg and keep your core tight."
  ]
  
  pipe = StableDiffusionPipeline.from_pretrained(
      "stabilityai/stable-diffusion-xl-base-1.0",
      torch_dtype=torch.float16 if device=="cuda" else torch.float32
  ).to(device)
  
  frame_paths = []
  for i, pose in enumerate(pose_list):
      prompt = f"{character}, {pose}, realistic, high quality, full body"
      print(f"Generating frame {i+1} for prompt: {prompt}")
      image = pipe(prompt, num_inference_steps=25).images[0]
      frame_path = os.path.join(frames_dir, f"frame_{i+1}.png")
      image.save(frame_path)
      frame_paths.append(frame_path)
  ```
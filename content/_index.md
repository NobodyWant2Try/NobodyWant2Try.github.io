---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-17
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
        skills: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I have worked on 3D Gaussian Splatting, 3D Reconstruction and Rendering.

        These days, I'm studying Multimodal LLMs and Embodied AI.

        In the fueature, I'll learn more about LLMs and RL.

        Please reach out to collaborate 😃
    design:
      columns: '1'
  - block: collection
    id: news
    content:
      title: News
      filters:
        folders:
          - blog      # 直接从 blog 文件夹读
        exclude_future: false
        exclude_past: false
      count: 10
      order: desc
    design:
      view: card
  - block: collection
    id: projects
    content:
      title: Projects
      text: ''
      filters:
        folders:
          - projects
        exclude_featured: false
      count: 4     # 最多展示几个项目
      order: desc
    design:
      view: card    # 项目卡片风格，也可以用 showcase 等
      columns: 4
      spacing:
        padding: ['2rem', '0', '2rem', '0']
---

# profile
runtime: php55

handlers:
- url: /styles
  static_dir: styles
  
- url: /images/(.*\.(gif|png|jpg))
  static_files: images/\1
  upload: images/(.*\.(gif|png|jpg))
  
- url: /.*
  script: index.html

app:
  description: ''
  icon: 🤖
  icon_background: '#FFEAD5'
  mode: workflow
  name: '11'
  use_icon_as_answer_icon: false
dependencies:
- current_identifier: null
  type: marketplace
  value:
    marketplace_plugin_unique_identifier: langgenius/mineru:0.2.0@24558d66a86115cd8ace5e14fc4b22739a9a27ce71043e1066dae9d0ac126198
kind: app
version: 0.3.0
workflow:
  conversation_variables: []
  environment_variables: []
  features:
    file_upload:
      allowed_file_extensions:
      - .JPG
      - .JPEG
      - .PNG
      - .GIF
      - .WEBP
      - .SVG
      allowed_file_types:
      - image
      allowed_file_upload_methods:
      - local_file
      - remote_url
      enabled: false
      fileUploadConfig:
        audio_file_size_limit: 50
        batch_count_limit: 5
        file_size_limit: 15
        image_file_size_limit: 10
        video_file_size_limit: 100
        workflow_file_upload_limit: 10
      image:
        enabled: false
        number_limits: 3
        transfer_methods:
        - local_file
        - remote_url
      number_limits: 3
    opening_statement: ''
    retriever_resource:
      enabled: true
    sensitive_word_avoidance:
      enabled: false
    speech_to_text:
      enabled: false
    suggested_questions: []
    suggested_questions_after_answer:
      enabled: false
    text_to_speech:
      enabled: false
      language: ''
      voice: ''
  graph:
    edges:
    - data:
        isInIteration: false
        isInLoop: false
        sourceType: start
        targetType: tool
      id: 1751548070751-source-1751553629165-target
      source: '1751548070751'
      sourceHandle: source
      target: '1751553629165'
      targetHandle: target
      type: custom
      zIndex: 0
    - data:
        isInIteration: false
        isInLoop: false
        sourceType: tool
        targetType: end
      id: 1751553629165-source-1751554193986-target
      source: '1751553629165'
      sourceHandle: source
      target: '1751554193986'
      targetHandle: target
      type: custom
      zIndex: 0
    nodes:
    - data:
        desc: ''
        selected: false
        title: 开始
        type: start
        variables:
        - allowed_file_extensions: []
          allowed_file_types:
          - document
          allowed_file_upload_methods:
          - local_file
          - remote_url
          label: tt
          max_length: 48
          options: []
          required: true
          type: file
          variable: tt
      height: 89
      id: '1751548070751'
      position:
        x: 30
        y: 322.5
      positionAbsolute:
        x: 30
        y: 322.5
      selected: false
      sourcePosition: right
      targetPosition: left
      type: custom
      width: 244
    - data:
        desc: ''
        is_team_authorization: true
        output_schema:
          properties:
            full_zip_url:
              description: The zip URL of the complete parsed result
              type: string
            images:
              description: The images extracted from the file
              items:
                type: object
              type: array
          type: object
        paramSchemas:
        - auto_generate: null
          default: null
          form: llm
          human_description:
            en_US: the file to be parsed(support pdf, ppt, pptx, doc, docx, png, jpg,
              jpeg)
            ja_JP: 解析するファイル(pdf、ppt、pptx、doc、docx、png、jpg、jpegをサポート)
            pt_BR: the file to be parsed(support pdf, ppt, pptx, doc, docx, png, jpg,
              jpeg)
            zh_Hans: 用于解析的文件(支持 pdf, ppt, pptx, doc, docx, png, jpg, jpeg)
          label:
            en_US: file
            ja_JP: file
            pt_BR: file
            zh_Hans: file
          llm_description: the file to be parsed (support pdf, ppt, pptx, doc, docx,
            png, jpg, jpeg)
          max: null
          min: null
          name: file
          options: []
          placeholder: null
          precision: null
          required: true
          scope: null
          template: null
          type: file
        - auto_generate: null
          default: auto
          form: form
          human_description:
            en_US: (For local deployment service)Parsing method, can be auto, ocr,
              or txt. Default is auto. If results are not satisfactory, try ocr
            ja_JP: （ローカルデプロイメントサービス用）解析方法は、auto、ocr、またはtxtのいずれかです。デフォルトはautoです。結果が満足できない場合は、ocrを試してください
            pt_BR: (For local deployment service)Parsing method, can be auto, ocr,
              or txt. Default is auto. If results are not satisfactory, try ocr
            zh_Hans: （用于本地部署服务）解析方法，可以是auto, ocr, 或 txt。默认是auto。如果结果不理想，请尝试ocr
          label:
            en_US: parse method
            ja_JP: 解析方法
            pt_BR: parse method
            zh_Hans: 解析方法
          llm_description: Parsing method, can be auto, ocr, or txt. Default is auto.
            If results are not satisfactory, try ocr
          max: null
          min: null
          name: parse_method
          options:
          - icon: ''
            label:
              en_US: auto
              ja_JP: auto
              pt_BR: auto
              zh_Hans: auto
            value: auto
          - icon: ''
            label:
              en_US: ocr
              ja_JP: ocr
              pt_BR: ocr
              zh_Hans: ocr
            value: ocr
          - icon: ''
            label:
              en_US: txt
              ja_JP: txt
              pt_BR: txt
              zh_Hans: txt
            value: txt
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: select
        - auto_generate: null
          default: 1
          form: form
          human_description:
            en_US: (For official API) Whether to enable formula recognition
            ja_JP: （公式API用）数式認識を有効にするかどうか
            pt_BR: (For official API) Whether to enable formula recognition
            zh_Hans: （用于官方API）是否开启公式识别
          label:
            en_US: Enable formula recognition
            ja_JP: 数式認識を有効にする
            pt_BR: Enable formula recognition
            zh_Hans: 开启公式识别
          llm_description: (For official API) Whether to enable formula recognition
          max: null
          min: null
          name: enable_formula
          options: []
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: boolean
        - auto_generate: null
          default: 1
          form: form
          human_description:
            en_US: (For official API) Whether to enable table recognition
            ja_JP: （公式API用）表認識を有効にするかどうか
            pt_BR: (For official API) Whether to enable table recognition
            zh_Hans: （用于官方API）是否开启表格识别
          label:
            en_US: Enable table recognition
            ja_JP: 表認識を有効にする
            pt_BR: Enable table recognition
            zh_Hans: 开启表格识别
          llm_description: (For official API) Whether to enable table recognition
          max: null
          min: null
          name: enable_table
          options: []
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: boolean
        - auto_generate: null
          default: doclayout_yolo
          form: form
          human_description:
            en_US: '(For official API) Optional values: doclayout_yolo, layoutlmv3,
              default value is doclayout_yolo. doclayout_yolo is a self-developed
              model with better effect'
            ja_JP: （公式API用）オプション値：doclayout_yolo、layoutlmv3、デフォルト値は doclayout_yolo。doclayout_yolo
              は自己開発モデルで、効果がより良い
            pt_BR: '(For official API) Optional values: doclayout_yolo, layoutlmv3,
              default value is doclayout_yolo. doclayout_yolo is a self-developed
              model with better effect'
            zh_Hans: （用于官方API）可选值：doclayout_yolo、layoutlmv3，默认值为 doclayout_yolo。doclayout_yolo
              为自研模型，效果更好
          label:
            en_US: Layout model
            ja_JP: レイアウト検出モデル
            pt_BR: Layout model
            zh_Hans: 布局检测模型
          llm_description: '(For official API) Optional values: doclayout_yolo, layoutlmv3,
            default value is doclayout_yolo. doclayout_yolo is a self-developed model
            withbetter effect'
          max: null
          min: null
          name: layout_model
          options:
          - icon: ''
            label:
              en_US: doclayout_yolo
              ja_JP: doclayout_yolo
              pt_BR: doclayout_yolo
              zh_Hans: doclayout_yolo
            value: doclayout_yolo
          - icon: ''
            label:
              en_US: layoutlmv3
              ja_JP: layoutlmv3
              pt_BR: layoutlmv3
              zh_Hans: layoutlmv3
            value: layoutlmv3
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: select
        - auto_generate: null
          default: auto
          form: form
          human_description:
            en_US: '(For official API) Specify document language, default ch, can
              be set to auto, when auto, the model will automatically identify document
              language, other optional value list see: https://paddlepaddle.github.io/PaddleOCR/latest/ppocr/blog/multi_languages.html#5'
            ja_JP: （公式API用）ドキュメント言語を指定します。デフォルトはchで、autoに設定できます。autoの場合、モデルはドキュメント言語を自動的に識別します。他のオプション値リストについては、次を参照してください：https://paddlepaddle.github.io/PaddleOCR/latest/ppocr/blog/multi_languages.html#5
            pt_BR: '(For official API) Specify document language, default ch, can
              be set to auto, when auto, the model will automatically identify document
              language, other optional value list see: https://paddlepaddle.github.io/PaddleOCR/latest/ppocr/blog/multi_languages.html#5'
            zh_Hans: （用于官方API）指定文档语言，默认 ch，可以设置为auto，当为auto时模型会自动识别文档语言，其他可选值列表详见：https://paddlepaddle.github.io/PaddleOCR/latest/ppocr/blog/multi_languages.html#5
          label:
            en_US: Document language
            ja_JP: ドキュメント言語
            pt_BR: Document language
            zh_Hans: 文档语言
          llm_description: '(For official API) Specify document language, default
            ch, can be set to auto, when auto, the model will automatically identify
            document language, other optional value list see: https://paddlepaddle.github.io/PaddleOCR/latest/ppocr/blog/multi_languages.html#5'
          max: null
          min: null
          name: language
          options: []
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: string
        - auto_generate: null
          default: 0
          form: form
          human_description:
            en_US: (For official API) Whether to enable OCR recognition
            ja_JP: （公式API用）OCR認識を有効にするかどうか
            pt_BR: (For official API) Whether to enable OCR recognition
            zh_Hans: （用于官方API）是否开启OCR识别
          label:
            en_US: Enable OCR recognition
            ja_JP: OCR認識を有効にする
            pt_BR: Enable OCR recognition
            zh_Hans: 开启OCR识别
          llm_description: (For official API) Whether to enable OCR recognition
          max: null
          min: null
          name: enable_ocr
          options: []
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: boolean
        - auto_generate: null
          default: '[]'
          form: form
          human_description:
            en_US: '(For official API) Example: ["docx","html"], markdown, json are
              the default export formats, no need to set, this parameter only supports
              one or more of docx, html, latex'
            ja_JP: （公式API用）例：["docx","html"]、markdown、jsonはデフォルトのエクスポート形式であり、設定する必要はありません。このパラメータは、docx、html、latexの3つの形式のいずれかまたは複数のみをサポートします
            pt_BR: '(For official API) Example: ["docx","html"], markdown, json are
              the default export formats, no need to set, this parameter only supports
              one or more of docx, html, latex'
            zh_Hans: （用于官方API）示例：["docx","html"],markdown、json为默认导出格式，无须设置，该参数仅支持docx、html、latex三种格式中的一个或多个
          label:
            en_US: Extra export formats
            ja_JP: 追加のエクスポート形式
            pt_BR: Extra export formats
            zh_Hans: 额外导出格式
          llm_description: '(For official API) Example: ["docx","html"], markdown,
            json are the default export formats, no need to set, this parameter only
            supports one or more of docx, html, latex'
          max: null
          min: null
          name: extra_formats
          options: []
          placeholder: null
          precision: null
          required: false
          scope: null
          template: null
          type: string
        params:
          enable_formula: ''
          enable_ocr: ''
          enable_table: ''
          extra_formats: ''
          file: ''
          language: ''
          layout_model: ''
          parse_method: ''
        provider_id: langgenius/mineru/mineru
        provider_name: langgenius/mineru/mineru
        provider_type: builtin
        selected: false
        title: Parse File
        tool_configurations:
          enable_formula: 1
          enable_ocr: 0
          enable_table: 1
          extra_formats: '[]'
          language: auto
          layout_model: doclayout_yolo
          parse_method: auto
        tool_description: 一个用于解析文本，表格和图片的工具，支持pdf,pptx,docx等多种格式。支持英语，中文等多种语言
        tool_label: Parse File
        tool_name: parse-file
        tool_parameters:
          file:
            type: variable
            value:
            - '1751548070751'
            - tt
        type: tool
      height: 245
      id: '1751553629165'
      position:
        x: 334
        y: 322.5
      positionAbsolute:
        x: 334
        y: 322.5
      selected: false
      sourcePosition: right
      targetPosition: left
      type: custom
      width: 244
    - data:
        desc: ''
        outputs:
        - value_selector:
          - '1751553629165'
          - text
          value_type: string
          variable: text
        selected: true
        title: 结束
        type: end
      height: 89
      id: '1751554193986'
      position:
        x: 638
        y: 322.5
      positionAbsolute:
        x: 638
        y: 322.5
      sourcePosition: right
      targetPosition: left
      type: custom
      width: 244
    viewport:
      x: 270.99999999999994
      y: -9
      zoom: 0.7

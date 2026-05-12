{
  "data": {
    "edges": [
      {
        "animated": false,
        "className": "",
        "data": {
          "sourceHandle": {
            "dataType": "ChatInput",
            "id": "ChatInput-qnOgR",
            "name": "message",
            "output_types": [
              "Message"
            ]
          },
          "targetHandle": {
            "fieldName": "input_value",
            "id": "Agent-Axy3M",
            "inputTypes": [
              "Message"
            ],
            "type": "str"
          }
        },
        "id": "reactflow__edge-ChatInput-qnOgR{œdataTypeœ:œChatInputœ,œidœ:œChatInput-qnOgRœ,œnameœ:œmessageœ,œoutput_typesœ:[œMessageœ]}-Agent-Axy3M{œfieldNameœ:œinput_valueœ,œidœ:œAgent-Axy3Mœ,œinputTypesœ:[œMessageœ],œtypeœ:œstrœ}",
        "selected": false,
        "source": "ChatInput-qnOgR",
        "sourceHandle": "{œdataTypeœ:œChatInputœ,œidœ:œChatInput-qnOgRœ,œnameœ:œmessageœ,œoutput_typesœ:[œMessageœ]}",
        "target": "Agent-Axy3M",
        "targetHandle": "{œfieldNameœ:œinput_valueœ,œidœ:œAgent-Axy3Mœ,œinputTypesœ:[œMessageœ],œtypeœ:œstrœ}"
      },
      {
        "animated": false,
        "className": "",
        "data": {
          "sourceHandle": {
            "dataType": "Agent",
            "id": "Agent-Axy3M",
            "name": "response",
            "output_types": [
              "Message"
            ]
          },
          "targetHandle": {
            "fieldName": "input_value",
            "id": "ChatOutput-WZhCt",
            "inputTypes": [
              "Data",
              "DataFrame",
              "Message"
            ],
            "type": "other"
          }
        },
        "id": "reactflow__edge-Agent-Axy3M{œdataTypeœ:œAgentœ,œidœ:œAgent-Axy3Mœ,œnameœ:œresponseœ,œoutput_typesœ:[œMessageœ]}-ChatOutput-WZhCt{œfieldNameœ:œinput_valueœ,œidœ:œChatOutput-WZhCtœ,œinputTypesœ:[œDataœ,œDataFrameœ,œMessageœ],œtypeœ:œotherœ}",
        "selected": false,
        "source": "Agent-Axy3M",
        "sourceHandle": "{œdataTypeœ:œAgentœ,œidœ:œAgent-Axy3Mœ,œnameœ:œresponseœ,œoutput_typesœ:[œMessageœ]}",
        "target": "ChatOutput-WZhCt",
        "targetHandle": "{œfieldNameœ:œinput_valueœ,œidœ:œChatOutput-WZhCtœ,œinputTypesœ:[œDataœ,œDataFrameœ,œMessageœ],œtypeœ:œotherœ}"
      },
      {
        "animated": false,
        "className": "",
        "data": {
          "sourceHandle": {
            "dataType": "AIGCIwriteProcessor",
            "id": "AIGCIwriteProcessor-zTx6J",
            "name": "component_as_tool",
            "output_types": [
              "Tool"
            ]
          },
          "targetHandle": {
            "fieldName": "tools",
            "id": "Agent-Axy3M",
            "inputTypes": [
              "Tool"
            ],
            "type": "other"
          }
        },
        "id": "xy-edge__AIGCIwriteProcessor-zTx6J{œdataTypeœ:œAIGCIwriteProcessorœ,œidœ:œAIGCIwriteProcessor-zTx6Jœ,œnameœ:œcomponent_as_toolœ,œoutput_typesœ:[œToolœ]}-Agent-Axy3M{œfieldNameœ:œtoolsœ,œidœ:œAgent-Axy3Mœ,œinputTypesœ:[œToolœ],œtypeœ:œotherœ}",
        "selected": false,
        "source": "AIGCIwriteProcessor-zTx6J",
        "sourceHandle": "{œdataTypeœ:œAIGCIwriteProcessorœ,œidœ:œAIGCIwriteProcessor-zTx6Jœ,œnameœ:œcomponent_as_toolœ,œoutput_typesœ:[œToolœ]}",
        "target": "Agent-Axy3M",
        "targetHandle": "{œfieldNameœ:œtoolsœ,œidœ:œAgent-Axy3Mœ,œinputTypesœ:[œToolœ],œtypeœ:œotherœ}"
      }
    ],
    "nodes": [
      {
        "data": {
          "id": "ChatInput-qnOgR",
          "node": {
            "base_classes": [
              "Message"
            ],
            "beta": false,
            "conditional_paths": [],
            "custom_fields": {},
            "description": "从操作区获取聊天输入。",
            "display_name": "聊天输入",
            "documentation": "",
            "edited": false,
            "field_order": [
              "input_value",
              "should_store_message",
              "sender",
              "sender_name",
              "session_id",
              "files",
              "background_color",
              "chat_icon",
              "text_color"
            ],
            "frozen": false,
            "icon": "MessagesSquare",
            "legacy": false,
            "lf_version": "",
            "metadata": {},
            "minimized": true,
            "output_types": [],
            "outputs": [
              {
                "allows_loop": false,
                "cache": true,
                "display_name": "Chat Message",
                "group_outputs": false,
                "method": "message_response",
                "name": "message",
                "selected": "Message",
                "tool_mode": true,
                "types": [
                  "Message"
                ],
                "value": "__UNDEFINED__"
              }
            ],
            "pinned": false,
            "template": {
              "_type": "Component",
              "background_color": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "背景颜色",
                "dynamic": false,
                "info": "图标的背景颜色。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "background_color",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "chat_icon": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "图标",
                "dynamic": false,
                "info": "消息的图标。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "chat_icon",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "code": {
                "advanced": true,
                "dynamic": true,
                "fileTypes": [],
                "file_path": "",
                "info": "",
                "list": false,
                "load_from_db": false,
                "multiline": true,
                "name": "code",
                "password": false,
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "type": "code",
                "value": "from langflow.base.data.utils import IMG_FILE_TYPES, TEXT_FILE_TYPES\nfrom langflow.base.io.chat import ChatComponent\nfrom langflow.inputs import BoolInput\nfrom langflow.io import (\n    DropdownInput,\n    FileInput,\n    MessageTextInput,\n    MultilineInput,\n    Output,\n)\nfrom langflow.schema.message import Message\nfrom langflow.utils.constants import (\n    MESSAGE_SENDER_AI,\n    MESSAGE_SENDER_NAME_USER,\n    MESSAGE_SENDER_USER,\n)\n\n\nclass ChatInput(ChatComponent):\n    display_name = \"Chat Input\"\n    description = \"Get chat inputs from the Playground.\"\n    icon = \"MessagesSquare\"\n    name = \"ChatInput\"\n    minimized = True\n\n    inputs = [\n        MultilineInput(\n            name=\"input_value\",\n            display_name=\"Input Text\",\n            value=\"\",\n            info=\"Message to be passed as input.\",\n            input_types=[],\n        ),\n        BoolInput(\n            name=\"should_store_message\",\n            display_name=\"Store Messages\",\n            info=\"Store the message in the history.\",\n            value=True,\n            advanced=True,\n        ),\n        DropdownInput(\n            name=\"sender\",\n            display_name=\"Sender Type\",\n            options=[MESSAGE_SENDER_AI, MESSAGE_SENDER_USER],\n            value=MESSAGE_SENDER_USER,\n            info=\"Type of sender.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"sender_name\",\n            display_name=\"Sender Name\",\n            info=\"Name of the sender.\",\n            value=MESSAGE_SENDER_NAME_USER,\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"session_id\",\n            display_name=\"Session ID\",\n            info=\"The session ID of the chat. If empty, the current session ID parameter will be used.\",\n            advanced=True,\n        ),\n        FileInput(\n            name=\"files\",\n            display_name=\"Files\",\n            file_types=TEXT_FILE_TYPES + IMG_FILE_TYPES,\n            info=\"Files to be sent with the message.\",\n            advanced=True,\n            is_list=True,\n            temp_file=True,\n        ),\n        MessageTextInput(\n            name=\"background_color\",\n            display_name=\"Background Color\",\n            info=\"The background color of the icon.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"chat_icon\",\n            display_name=\"Icon\",\n            info=\"The icon of the message.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"text_color\",\n            display_name=\"Text Color\",\n            info=\"The text color of the name\",\n            advanced=True,\n        ),\n    ]\n    outputs = [\n        Output(display_name=\"Chat Message\", name=\"message\", method=\"message_response\"),\n    ]\n\n    async def message_response(self) -> Message:\n        background_color = self.background_color\n        text_color = self.text_color\n        icon = self.chat_icon\n\n        message = await Message.create(\n            text=self.input_value,\n            sender=self.sender,\n            sender_name=self.sender_name,\n            session_id=self.session_id,\n            files=self.files,\n            properties={\n                \"background_color\": background_color,\n                \"text_color\": text_color,\n                \"icon\": icon,\n            },\n        )\n        if self.session_id and isinstance(message, Message) and self.should_store_message:\n            stored_message = await self.send_message(\n                message,\n            )\n            self.message.value = stored_message\n            message = stored_message\n\n        self.status = message\n        return message\n"
              },
              "files": {
                "_input_type": "FileInput",
                "advanced": true,
                "display_name": "文件",
                "dynamic": false,
                "fileTypes": [
                  "txt",
                  "md",
                  "mdx",
                  "csv",
                  "json",
                  "yaml",
                  "yml",
                  "xml",
                  "html",
                  "htm",
                  "pdf",
                  "docx",
                  "py",
                  "sh",
                  "sql",
                  "js",
                  "ts",
                  "tsx",
                  "jpg",
                  "jpeg",
                  "png",
                  "bmp",
                  "image"
                ],
                "file_path": "",
                "info": "随消息发送的文件。",
                "list": true,
                "list_add_label": "Add More",
                "name": "files",
                "placeholder": "",
                "required": false,
                "show": true,
                "temp_file": true,
                "title_case": false,
                "trace_as_metadata": true,
                "type": "file",
                "value": ""
              },
              "input_value": {
                "_input_type": "MultilineInput",
                "advanced": false,
                "copy_field": false,
                "display_name": "输入文本",
                "dynamic": false,
                "info": "作为输入传递的消息。",
                "input_types": [],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "multiline": true,
                "name": "input_value",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "1. 意图分类（面试模式 vs. 普通对话）\n\n智能体需区分三种用户输入类型：\n类型\t触发条件\t示例\n开始面试\t用户消息包含 \"start interview\", \"begin\", \"开始面试\", \"practice interview\", \"let's practice\"\t“Let’s start the interview.”\n面试回答\t智能体已处于面试模式，并且用户消息长度 ≥ 5 个单词（或包含完整句子）\t“My name is Li Ming, and I am a computer science major.”\n普通对话/提问\t用户消息很短（如 “Hi”, “What can you do?”），或询问与面试无关的内容（如 “Tell me a joke”）\t“Can you repeat the question?” 也归类为面试中的请求，而非独立对话\n\n    规则：一旦进入“面试模式”，除非用户明确说 “stop” / “end interview” / “退出”，否则后续所有长消息（≥5词）都优先视为对当前问题的回答。\n    若用户在面试模式下提问（如 “What does ‘strength’ mean?”），则进入“帮助/解释”子模式，解答后恢复面试。\n\n2. 内容提取（从用户回答中提取有效文本）\n\n当判定用户消息为“面试回答”时，执行以下提取步骤：\n\n    移除元对话标记：\n    删除用户消息中的 “My answer is:”, “Here is my response:”, “Answer:” 等前缀，只保留之后的英文句子。\n\n    过滤填充词与重复（仅用于分析，不改变原显示）：\n    识别 um, uh, like, you know 等填充词，在反馈中可提示减少，但不从回答中删除（保持原样展示）。\n\n    清洗标点与格式：\n\n        将所有中文标点（，。！？）替换为英文（, . ! ?）\n\n        移除多余空格和换行\n\n    长度校验：\n\n        若清理后的回答 单词数 < 5 → 触发 鼓励详细回答 提示：\n        “<span style=\"color:blue\">Could you please say a little more? Try to make a complete sentence.</span>”\n\n        若单词数在 5~20 之间 → 正常进入反馈，但追问中建议扩展\n\n        若单词数 ≥ 20 → 直接进入评估与反馈\n\n3. 特殊情况处理\n用户输入\t智能体行为\n“I don’t know” / “I’m not sure”\t不视为无效回答，而是给出鼓励和示例引导：\n“No problem. You could say: ‘I haven’t faced that situation yet, but I would...’ Would you like to try again?”\n“Can you repeat the question?”\t重复上一问题（不扣分）\n“What does XYZ mean?” (例如 “What does ‘teamwork’ mean?”)\t用简单英语解释词汇，然后重新问原问题\n用户回答中掺杂中文\t保留中文原样，但在反馈中提供完整英文示范回答，并温和建议：\n“Try to use English as much as possible. Here’s an example: ...”\n4. 上下文关联（多轮追问检测）\n\n智能体需记录以下上下文变量：\n\n    current_question：当前面试题目（字符串）\n\n    last_user_answer：用户最近一次回答（清洗后的文本）\n\n    follow_up_count：针对当前主问题的已追问次数（上限 2 次）\n\n当用户在新一轮输入后，若 follow_up_count < 2 且回答内容明显不完整（缺少例子、理由或结果），则自动生成一次追问，而不是直接给反馈。\n\n判断“回答不完整”的简单规则：\n\n    不包含 “because”, “for example”, “such as” 等扩展词\n\n    句子总数 ≤ 2 句\n\n    没有提及任何具体经历或结果\n\n    示例：\n    问题：“What is your greatest strength?”\n    用户回答：“I am hard-working.” → 不完整（无例子） → 追问：“Can you give me an example of when you worked hard?”\n\n5. 输入示例与提取结果\n示例1（开始面试）\n\n用户：“Hi, I want to practice interview. Start please.”\n提取结果：type = “start_interview” → 智能体输出第一个问题。\n示例2（面试回答 + 元标记）\n\n用户：“My answer is: I study nursing because I like helping people.”\n提取结果：cleaned_answer = “I study nursing because I like helping people.”\n单词数：8 → 正常进入反馈。\n示例3（面试回答 + 填充词）\n\n用户：“Um, I think, like, my strength is I’m very responsible.”\n提取结果：保留原文，但在反馈中提示减少填充词。\n示例4（普通对话）\n\n用户：“Hello” （且未处于面试模式）\n提取结果：type = “normal_chat” → 智能体回复：“Hello! Would you like to start an interview practice?”"
              },
              "sender": {
                "_input_type": "DropdownInput",
                "advanced": true,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "发送者类型",
                "dynamic": false,
                "info": "发送者类型。",
                "name": "sender",
                "options": [
                  "Machine",
                  "User"
                ],
                "options_metadata": [],
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "str",
                "value": "User"
              },
              "sender_name": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "发送者名称",
                "dynamic": false,
                "info": "发送者名称。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "sender_name",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "User"
              },
              "session_id": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "会话 ID",
                "dynamic": false,
                "info": "聊天的会话 ID。如果为空，则将使用当前会话 ID 参数。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "session_id",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "should_store_message": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "存储消息",
                "dynamic": false,
                "info": "将消息存储在历史记录中。",
                "list": false,
                "list_add_label": "Add More",
                "name": "should_store_message",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              },
              "text_color": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "文本颜色",
                "dynamic": false,
                "info": "名称的文本颜色",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "text_color",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              }
            },
            "tool_mode": false
          },
          "type": "ChatInput"
        },
        "dragging": false,
        "id": "ChatInput-qnOgR",
        "measured": {
          "height": 203,
          "width": 320
        },
        "position": {
          "x": 808.0025929771274,
          "y": 593.1928838597865
        },
        "selected": false,
        "type": "genericNode"
      },
      {
        "data": {
          "description": "Display a chat message in the Playground.",
          "display_name": "Chat Output",
          "id": "ChatOutput-WZhCt",
          "node": {
            "base_classes": [
              "Message"
            ],
            "beta": false,
            "conditional_paths": [],
            "custom_fields": {},
            "description": "在操作区显示聊天消息。",
            "display_name": "聊天输出",
            "documentation": "",
            "edited": false,
            "field_order": [
              "input_value",
              "should_store_message",
              "sender",
              "sender_name",
              "session_id",
              "data_template",
              "background_color",
              "chat_icon",
              "text_color",
              "clean_data"
            ],
            "frozen": false,
            "icon": "MessagesSquare",
            "legacy": false,
            "lf_version": "",
            "metadata": {},
            "minimized": true,
            "output_types": [],
            "outputs": [
              {
                "allows_loop": false,
                "cache": true,
                "display_name": "Output Message",
                "group_outputs": false,
                "method": "message_response",
                "name": "message",
                "selected": "Message",
                "tool_mode": true,
                "types": [
                  "Message"
                ],
                "value": "__UNDEFINED__"
              }
            ],
            "pinned": false,
            "template": {
              "_type": "Component",
              "background_color": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "背景颜色",
                "dynamic": false,
                "info": "图标的背景颜色。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "background_color",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "chat_icon": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "图标",
                "dynamic": false,
                "info": "消息的图标。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "chat_icon",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "clean_data": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "基本清理数据",
                "dynamic": false,
                "info": "是否清理数据",
                "list": false,
                "list_add_label": "Add More",
                "name": "clean_data",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              },
              "code": {
                "advanced": true,
                "dynamic": true,
                "fileTypes": [],
                "file_path": "",
                "info": "",
                "list": false,
                "load_from_db": false,
                "multiline": true,
                "name": "code",
                "password": false,
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "type": "code",
                "value": "from collections.abc import Generator\nfrom typing import Any\n\nimport orjson\nfrom fastapi.encoders import jsonable_encoder\n\nfrom langflow.base.io.chat import ChatComponent\nfrom langflow.helpers.data import safe_convert\nfrom langflow.inputs import BoolInput\nfrom langflow.inputs.inputs import HandleInput\nfrom langflow.io import DropdownInput, MessageTextInput, Output\nfrom langflow.schema.data import Data\nfrom langflow.schema.dataframe import DataFrame\nfrom langflow.schema.message import Message\nfrom langflow.schema.properties import Source\nfrom langflow.utils.constants import (\n    MESSAGE_SENDER_AI,\n    MESSAGE_SENDER_NAME_AI,\n    MESSAGE_SENDER_USER,\n)\n\n\nclass ChatOutput(ChatComponent):\n    display_name = \"Chat Output\"\n    description = \"Display a chat message in the Playground.\"\n    icon = \"MessagesSquare\"\n    name = \"ChatOutput\"\n    minimized = True\n\n    inputs = [\n        HandleInput(\n            name=\"input_value\",\n            display_name=\"Inputs\",\n            info=\"Message to be passed as output.\",\n            input_types=[\"Data\", \"DataFrame\", \"Message\"],\n            required=True,\n        ),\n        BoolInput(\n            name=\"should_store_message\",\n            display_name=\"Store Messages\",\n            info=\"Store the message in the history.\",\n            value=True,\n            advanced=True,\n        ),\n        DropdownInput(\n            name=\"sender\",\n            display_name=\"Sender Type\",\n            options=[MESSAGE_SENDER_AI, MESSAGE_SENDER_USER],\n            value=MESSAGE_SENDER_AI,\n            advanced=True,\n            info=\"Type of sender.\",\n        ),\n        MessageTextInput(\n            name=\"sender_name\",\n            display_name=\"Sender Name\",\n            info=\"Name of the sender.\",\n            value=MESSAGE_SENDER_NAME_AI,\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"session_id\",\n            display_name=\"Session ID\",\n            info=\"The session ID of the chat. If empty, the current session ID parameter will be used.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"data_template\",\n            display_name=\"Data Template\",\n            value=\"{text}\",\n            advanced=True,\n            info=\"Template to convert Data to Text. If left empty, it will be dynamically set to the Data's text key.\",\n        ),\n        MessageTextInput(\n            name=\"background_color\",\n            display_name=\"Background Color\",\n            info=\"The background color of the icon.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"chat_icon\",\n            display_name=\"Icon\",\n            info=\"The icon of the message.\",\n            advanced=True,\n        ),\n        MessageTextInput(\n            name=\"text_color\",\n            display_name=\"Text Color\",\n            info=\"The text color of the name\",\n            advanced=True,\n        ),\n        BoolInput(\n            name=\"clean_data\",\n            display_name=\"Basic Clean Data\",\n            value=True,\n            info=\"Whether to clean the data\",\n            advanced=True,\n        ),\n    ]\n    outputs = [\n        Output(\n            display_name=\"Output Message\",\n            name=\"message\",\n            method=\"message_response\",\n        ),\n    ]\n\n    def _build_source(self, id_: str | None, display_name: str | None, source: str | None) -> Source:\n        source_dict = {}\n        if id_:\n            source_dict[\"id\"] = id_\n        if display_name:\n            source_dict[\"display_name\"] = display_name\n        if source:\n            # Handle case where source is a ChatOpenAI object\n            if hasattr(source, \"model_name\"):\n                source_dict[\"source\"] = source.model_name\n            elif hasattr(source, \"model\"):\n                source_dict[\"source\"] = str(source.model)\n            else:\n                source_dict[\"source\"] = str(source)\n        return Source(**source_dict)\n\n    async def message_response(self) -> Message:\n        # First convert the input to string if needed\n        text = self.convert_to_string()\n\n        # Get source properties\n        source, icon, display_name, source_id = self.get_properties_from_source_component()\n        background_color = self.background_color\n        text_color = self.text_color\n        if self.chat_icon:\n            icon = self.chat_icon\n\n        # Create or use existing Message object\n        if isinstance(self.input_value, Message):\n            message = self.input_value\n            # Update message properties\n            message.text = text\n        else:\n            message = Message(text=text)\n\n        # Set message properties\n        message.sender = self.sender\n        message.sender_name = self.sender_name\n        message.session_id = self.session_id\n        message.flow_id = self.graph.flow_id if hasattr(self, \"graph\") else None\n        message.properties.source = self._build_source(source_id, display_name, source)\n        message.properties.icon = icon\n        message.properties.background_color = background_color\n        message.properties.text_color = text_color\n\n        # Store message if needed\n        if self.session_id and self.should_store_message:\n            stored_message = await self.send_message(message)\n            self.message.value = stored_message\n            message = stored_message\n\n        self.status = message\n        return message\n\n    def _serialize_data(self, data: Data) -> str:\n        \"\"\"Serialize Data object to JSON string.\"\"\"\n        # Convert data.data to JSON-serializable format\n        serializable_data = jsonable_encoder(data.data)\n        # Serialize with orjson, enabling pretty printing with indentation\n        json_bytes = orjson.dumps(serializable_data, option=orjson.OPT_INDENT_2)\n        # Convert bytes to string and wrap in Markdown code blocks\n        return \"```json\\n\" + json_bytes.decode(\"utf-8\") + \"\\n```\"\n\n    def _validate_input(self) -> None:\n        \"\"\"Validate the input data and raise ValueError if invalid.\"\"\"\n        if self.input_value is None:\n            msg = \"Input data cannot be None\"\n            raise ValueError(msg)\n        if isinstance(self.input_value, list) and not all(\n            isinstance(item, Message | Data | DataFrame | str) for item in self.input_value\n        ):\n            invalid_types = [\n                type(item).__name__\n                for item in self.input_value\n                if not isinstance(item, Message | Data | DataFrame | str)\n            ]\n            msg = f\"Expected Data or DataFrame or Message or str, got {invalid_types}\"\n            raise TypeError(msg)\n        if not isinstance(\n            self.input_value,\n            Message | Data | DataFrame | str | list | Generator | type(None),\n        ):\n            type_name = type(self.input_value).__name__\n            msg = f\"Expected Data or DataFrame or Message or str, Generator or None, got {type_name}\"\n            raise TypeError(msg)\n\n    def convert_to_string(self) -> str | Generator[Any, None, None]:\n        \"\"\"Convert input data to string with proper error handling.\"\"\"\n        self._validate_input()\n        if isinstance(self.input_value, list):\n            return \"\\n\".join([safe_convert(item, clean_data=self.clean_data) for item in self.input_value])\n        if isinstance(self.input_value, Generator):\n            return self.input_value\n        return safe_convert(self.input_value)\n"
              },
              "data_template": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "数据模板",
                "dynamic": false,
                "info": "将数据转换为文本的模板。如果留空，它将动态设置为数据的文本键。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "data_template",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "{text}"
              },
              "input_value": {
                "_input_type": "HandleInput",
                "advanced": false,
                "display_name": "输入",
                "dynamic": false,
                "info": "作为输出传递的消息。",
                "input_types": [
                  "Data",
                  "DataFrame",
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "name": "input_value",
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "trace_as_metadata": true,
                "type": "other",
                "value": ""
              },
              "sender": {
                "_input_type": "DropdownInput",
                "advanced": true,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "发送者类型",
                "dynamic": false,
                "info": "发送者类型。",
                "name": "sender",
                "options": [
                  "Machine",
                  "User"
                ],
                "options_metadata": [],
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "str",
                "value": "Machine"
              },
              "sender_name": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "发送者名称",
                "dynamic": false,
                "info": "发送者名称。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "sender_name",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "AI"
              },
              "session_id": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "会话 ID",
                "dynamic": false,
                "info": "聊天的会话 ID。如果为空，则将使用当前会话 ID 参数。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "session_id",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "should_store_message": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "存储消息",
                "dynamic": false,
                "info": "将消息存储在历史记录中。",
                "list": false,
                "list_add_label": "Add More",
                "name": "should_store_message",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              },
              "text_color": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "文本颜色",
                "dynamic": false,
                "info": "名称的文本颜色",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "text_color",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              }
            },
            "tool_mode": false
          },
          "type": "ChatOutput"
        },
        "dragging": false,
        "id": "ChatOutput-WZhCt",
        "measured": {
          "height": 165,
          "width": 320
        },
        "position": {
          "x": 1834.5561653524628,
          "y": 353.01811794011115
        },
        "selected": false,
        "type": "genericNode"
      },
      {
        "data": {
          "id": "Agent-Axy3M",
          "node": {
            "base_classes": [
              "Message"
            ],
            "beta": false,
            "conditional_paths": [],
            "custom_fields": {},
            "description": "定义智能体的指令，然后输入任务以使用工具完成。",
            "display_name": "智能体",
            "documentation": "",
            "edited": false,
            "field_order": [
              "agent_llm",
              "max_tokens",
              "model_kwargs",
              "json_mode",
              "model_name",
              "temperature",
              "seed",
              "tool_calling",
              "model_name",
              "system_prompt",
              "tools",
              "input_value",
              "handle_parsing_errors",
              "verbose",
              "max_iterations",
              "agent_description",
              "memory",
              "sender",
              "sender_name",
              "n_messages",
              "session_id",
              "order",
              "template",
              "add_current_date_tool"
            ],
            "frozen": false,
            "icon": "bot",
            "legacy": false,
            "lf_version": "",
            "metadata": {},
            "minimized": false,
            "output_types": [],
            "outputs": [
              {
                "allows_loop": false,
                "cache": true,
                "display_name": "Response",
                "group_outputs": false,
                "method": "message_response",
                "name": "response",
                "selected": "Message",
                "tool_mode": true,
                "types": [
                  "Message"
                ],
                "value": "__UNDEFINED__"
              }
            ],
            "pinned": false,
            "template": {
              "_type": "Component",
              "add_current_date_tool": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "当前日期",
                "dynamic": false,
                "info": "如果为 true，将向智能体添加一个返回当前日期的工具。",
                "list": false,
                "list_add_label": "Add More",
                "name": "add_current_date_tool",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              },
              "agent_description": {
                "_input_type": "MultilineInput",
                "advanced": true,
                "copy_field": false,
                "display_name": "智能体描述 [已弃用]",
                "dynamic": false,
                "info": "智能体的描述。仅在工具模式下使用。默认为“一个可以访问以下工具的有用助手：”，并且工具是动态添加的。此功能已弃用，并将在未来版本中删除。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "multiline": true,
                "name": "agent_description",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "A helpful assistant with access to the following tools:"
              },
              "agent_llm": {
                "_input_type": "DropdownInput",
                "advanced": true,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "模型提供商",
                "dynamic": false,
                "info": "智能体将用于生成响应的语言模型的提供商。",
                "input_types": [],
                "name": "agent_llm",
                "options": [
                  "OpenAI"
                ],
                "options_metadata": [
                  {
                    "icon": "Amazon"
                  },
                  {
                    "icon": "Anthropic"
                  },
                  {
                    "icon": "Azure"
                  },
                  {
                    "icon": "GoogleGenerativeAI"
                  },
                  {
                    "icon": "Groq"
                  },
                  {
                    "icon": "NVIDIA"
                  },
                  {
                    "icon": "OpenAI"
                  },
                  {
                    "icon": "SambaNova"
                  },
                  {
                    "icon": "brain"
                  }
                ],
                "placeholder": "",
                "real_time_refresh": true,
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "str",
                "value": "OpenAI"
              },
              "code": {
                "advanced": true,
                "dynamic": true,
                "fileTypes": [],
                "file_path": "",
                "info": "",
                "list": false,
                "load_from_db": false,
                "multiline": true,
                "name": "code",
                "password": false,
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "type": "code",
                "value": "from typing import cast\nfrom langchain_core.tools import StructuredTool\n\nfrom langflow.base.agents.agent import LCToolsAgentComponent\nfrom langflow.base.agents.events import ExceptionWithMessageError\nfrom langflow.base.models.aigc_constants import AGENT_MODEL_NAMES\nfrom langflow.base.models.model_input_constants import (\n    ALL_PROVIDER_FIELDS,\n    MODEL_DYNAMIC_UPDATE_FIELDS,\n    MODEL_PROVIDERS_DICT,\n    MODELS_METADATA,\n)\nfrom langflow.base.models.model_utils import get_model_name\nfrom langflow.components.helpers import CurrentDateComponent\nfrom langflow.components.helpers.memory import MemoryComponent\nfrom langflow.components.langchain_utilities.tool_calling import ToolCallingAgentComponent\nfrom langflow.custom.custom_component.component import _get_component_toolkit\nfrom langflow.custom.utils import update_component_build_config\nfrom langflow.field_typing import Tool\nfrom langflow.io import BoolInput, DropdownInput, MultilineInput, Output\nfrom langflow.logging import logger\nfrom langflow.schema.dotdict import dotdict\nfrom langflow.schema.message import Message\n\n\ndef set_advanced_true(component_input):\n    component_input.advanced = True\n    return component_input\n\n\nclass AgentComponent(ToolCallingAgentComponent):\n    display_name: str = \"Agent\"\n    description: str = \"Define the agent's instructions, then enter a task to complete using tools.\"\n    icon = \"bot\"\n    beta = False\n    name = \"Agent\"\n\n    memory_inputs = [set_advanced_true(component_input) for component_input in MemoryComponent().inputs]\n\n    inputs = [\n        DropdownInput(\n            name=\"agent_llm\",\n            display_name=\"Model Provider\",\n            info=\"The provider of the language model that the agent will use to generate responses.\",\n            options=[\"OpenAI\"],\n            value=\"OpenAI\",\n            real_time_refresh=True,\n            input_types=[],\n            advanced=True,\n            options_metadata=[MODELS_METADATA[key] for key in sorted(MODELS_METADATA.keys())] + [{\"icon\": \"brain\"}],\n        ),\n        *MODEL_PROVIDERS_DICT[\"OpenAI\"][\"inputs\"],\n        DropdownInput(\n            name=\"model_name\",\n            display_name=\"Model Name\",\n            advanced=False,\n            options=AGENT_MODEL_NAMES,\n            value=AGENT_MODEL_NAMES[0],\n        ),\n        MultilineInput(\n            name=\"system_prompt\",\n            display_name=\"Agent Instructions\",\n            info=\"System Prompt: Initial instructions and context provided to guide the agent's behavior.\",\n            value=\"You are a helpful assistant that can use tools to answer questions and perform tasks.\",\n            advanced=False,\n        ),\n        *LCToolsAgentComponent._base_inputs,\n        *memory_inputs,\n        BoolInput(\n            name=\"add_current_date_tool\",\n            display_name=\"Current Date\",\n            advanced=True,\n            info=\"If true, will add a tool to the agent that returns the current date.\",\n            value=True,\n        ),\n    ]\n    outputs = [Output(name=\"response\", display_name=\"Response\", method=\"message_response\")]\n\n    async def message_response(self) -> Message:\n        try:\n            # Get LLM model and validate\n            llm_model, display_name = await self.get_llm()\n            if llm_model is None:\n                msg = \"No language model selected. Please choose a model to proceed.\"\n                raise ValueError(msg)\n            self.model_name = get_model_name(llm_model, display_name=display_name)\n\n            # Get memory data\n            self.chat_history = await self.get_memory_data()\n\n            # 这里的历史记录已包括了当前的输入值，所以需要删除最后一个\n            if self.chat_history:\n                last_msg = cast(Message, self.chat_history[-1])\n                if last_msg.sender == \"User\" and last_msg.text == self.input_value:\n                    self.chat_history.pop()\n\n            # Add current date tool if enabled\n            if self.add_current_date_tool:\n                if not isinstance(self.tools, list):  # type: ignore[has-type]\n                    self.tools = []\n                current_date_tool = (await CurrentDateComponent(**self.get_base_args()).to_toolkit()).pop(0)\n                if not isinstance(current_date_tool, StructuredTool):\n                    msg = \"CurrentDateComponent must be converted to a StructuredTool\"\n                    raise TypeError(msg)\n                self.tools.append(current_date_tool)\n\n            # Validate tools\n            if not self.tools:\n                msg = \"Tools are required to run the agent. Please add at least one tool.\"\n                raise ValueError(msg)\n\n            # Set up and run agent\n            self.set(\n                llm=llm_model,\n                tools=self.tools,\n                chat_history=self.chat_history,\n                input_value=self.input_value,\n                system_prompt=self.system_prompt,\n            )\n            agent = self.create_agent_runnable()\n            return await self.run_agent(agent)\n\n        except (ValueError, TypeError, KeyError) as e:\n            logger.error(f\"{type(e).__name__}: {e!s}\")\n            raise\n        except ExceptionWithMessageError as e:\n            logger.error(f\"ExceptionWithMessageError occurred: {e}\")\n            raise\n        except Exception as e:\n            logger.error(f\"Unexpected error: {e!s}\")\n            raise\n\n    async def get_memory_data(self):\n        memory_kwargs = {\n            component_input.name: getattr(self, f\"{component_input.name}\") for component_input in self.memory_inputs\n        }\n        # filter out empty values\n        memory_kwargs = {k: v for k, v in memory_kwargs.items() if v is not None}\n\n        return await MemoryComponent(**self.get_base_args()).set(**memory_kwargs).retrieve_messages()\n\n    async def get_llm(self):\n        if not isinstance(self.agent_llm, str):\n            return self.agent_llm, None\n\n        try:\n            provider_info = MODEL_PROVIDERS_DICT.get(self.agent_llm)\n            if not provider_info:\n                msg = f\"Invalid model provider: {self.agent_llm}\"\n                raise ValueError(msg)\n\n            component_class = provider_info.get(\"component_class\")\n            display_name = component_class.display_name\n            inputs = provider_info.get(\"inputs\")\n            prefix = provider_info.get(\"prefix\", \"\")\n\n            llm_model = await self._build_llm_model(component_class, inputs, prefix)\n            \n            # 确保LLM已经启用工具调用功能\n            if hasattr(llm_model, \"bind_tools\") and self.tools:\n                try:\n                    llm_model = llm_model.bind_tools(self.tools)\n                except Exception as e:\n                    logger.error(f\"Error binding tools to LLM: {e!s}\")\n                    msg = f\"Failed to bind tools to language model: {e!s}\"\n                    raise ValueError(msg) from e\n            \n            return llm_model, display_name\n\n        except Exception as e:\n            logger.error(f\"Error building {self.agent_llm} language model: {e!s}\")\n            msg = f\"Failed to initialize language model: {e!s}\"\n            raise ValueError(msg) from e\n\n    async def _build_llm_model(self, component, inputs, prefix=\"\"):\n        model_kwargs = {}\n        token = await self.get_variables(\"_aigc_token\", \"Token\")\n        userId = await self.get_variables(\"_aigc_userId\", \"UserId\")\n        for input_ in inputs:\n            if hasattr(self, f\"{prefix}{input_.name}\"):\n                model_kwargs[input_.name] = getattr(self, f\"{prefix}{input_.name}\")\n        \n        # 确保启用工具调用功能\n        model_kwargs[\"tool_calling\"] = True\n        \n        try:\n            # 构建模型\n            model = await component.set(**model_kwargs).build_model(token=token, userId=userId)\n            return model\n        except Exception as e:\n            logger.error(f\"Error building model: {e!s}\")\n            raise ValueError(f\"Failed to build model: {e!s}\") from e\n\n    def set_component_params(self, component):\n        provider_info = MODEL_PROVIDERS_DICT.get(self.agent_llm)\n        if provider_info:\n            inputs = provider_info.get(\"inputs\")\n            prefix = provider_info.get(\"prefix\")\n            model_kwargs = {input_.name: getattr(self, f\"{prefix}{input_.name}\") for input_ in inputs}\n\n            return component.set(**model_kwargs)\n        return component\n\n    def delete_fields(self, build_config: dotdict, fields: dict | list[str]) -> None:\n        \"\"\"Delete specified fields from build_config.\"\"\"\n        for field in fields:\n            build_config.pop(field, None)\n\n    def update_input_types(self, build_config: dotdict) -> dotdict:\n        \"\"\"Update input types for all fields in build_config.\"\"\"\n        for key, value in build_config.items():\n            if isinstance(value, dict):\n                if value.get(\"input_types\") is None:\n                    build_config[key][\"input_types\"] = []\n            elif hasattr(value, \"input_types\") and value.input_types is None:\n                value.input_types = []\n        return build_config\n\n    async def update_build_config(\n        self, build_config: dotdict, field_value: str, field_name: str | None = None\n    ) -> dotdict:\n        # Iterate over all providers in the MODEL_PROVIDERS_DICT\n        # Existing logic for updating build_config\n        if field_name in (\"agent_llm\",):\n            build_config[\"agent_llm\"][\"value\"] = field_value\n            provider_info = MODEL_PROVIDERS_DICT.get(field_value)\n            if provider_info:\n                component_class = provider_info.get(\"component_class\")\n                if component_class and hasattr(component_class, \"update_build_config\"):\n                    # Call the component class's update_build_config method\n                    build_config = await update_component_build_config(\n                        component_class, build_config, field_value, \"model_name\"\n                    )\n\n            provider_configs: dict[str, tuple[dict, list[dict]]] = {\n                provider: (\n                    MODEL_PROVIDERS_DICT[provider][\"fields\"],\n                    [\n                        MODEL_PROVIDERS_DICT[other_provider][\"fields\"]\n                        for other_provider in MODEL_PROVIDERS_DICT\n                        if other_provider != provider\n                    ],\n                )\n                for provider in MODEL_PROVIDERS_DICT\n            }\n            if field_value in provider_configs:\n                fields_to_add, fields_to_delete = provider_configs[field_value]\n\n                # Delete fields from other providers\n                for fields in fields_to_delete:\n                    self.delete_fields(build_config, fields)\n\n                # Add provider-specific fields\n                if field_value == \"OpenAI\" and not any(field in build_config for field in fields_to_add):\n                    build_config.update(fields_to_add)\n                else:\n                    build_config.update(fields_to_add)\n                # Reset input types for agent_llm\n                build_config[\"agent_llm\"][\"input_types\"] = []\n            elif field_value == \"Custom\":\n                # Delete all provider fields\n                self.delete_fields(build_config, ALL_PROVIDER_FIELDS)\n                # Update with custom component\n                custom_component = DropdownInput(\n                    name=\"agent_llm\",\n                    display_name=\"Language Model\",\n                    options=[*sorted(MODEL_PROVIDERS_DICT.keys()), \"Custom\"],\n                    value=\"Custom\",\n                    real_time_refresh=True,\n                    input_types=[\"LanguageModel\"],\n                    options_metadata=[MODELS_METADATA[key] for key in sorted(MODELS_METADATA.keys())]\n                    + [{\"icon\": \"brain\"}],\n                )\n                build_config.update({\"agent_llm\": custom_component.to_dict()})\n            # Update input types for all fields\n            build_config = self.update_input_types(build_config)\n\n            # Validate required keys\n            default_keys = [\n                \"code\",\n                \"_type\",\n                \"agent_llm\",\n                \"tools\",\n                \"input_value\",\n                \"add_current_date_tool\",\n                \"system_prompt\",\n                \"agent_description\",\n                \"max_iterations\",\n                \"handle_parsing_errors\",\n                \"verbose\",\n            ]\n            missing_keys = [key for key in default_keys if key not in build_config]\n            if missing_keys:\n                msg = f\"Missing required keys in build_config: {missing_keys}\"\n                raise ValueError(msg)\n        if (\n            isinstance(self.agent_llm, str)\n            and self.agent_llm in MODEL_PROVIDERS_DICT\n            and field_name in MODEL_DYNAMIC_UPDATE_FIELDS\n        ):\n            provider_info = MODEL_PROVIDERS_DICT.get(self.agent_llm)\n            if provider_info:\n                component_class = provider_info.get(\"component_class\")\n                component_class = self.set_component_params(component_class)\n                prefix = provider_info.get(\"prefix\")\n                if component_class and hasattr(component_class, \"update_build_config\"):\n                    # Call each component class's update_build_config method\n                    # remove the prefix from the field_name\n                    if isinstance(field_name, str) and isinstance(prefix, str):\n                        field_name = field_name.replace(prefix, \"\")\n                    build_config = await update_component_build_config(\n                        component_class, build_config, field_value, \"model_name\"\n                    )\n        return dotdict({k: v.to_dict() if hasattr(v, \"to_dict\") else v for k, v in build_config.items()})\n\n    async def _get_tools(self) -> list[Tool]:\n        component_toolkit = _get_component_toolkit()\n        tools_names = self._build_tools_names()\n        agent_description = self.get_tool_description()\n        # TODO: Agent Description Depreciated Feature to be removed\n        description = f\"{agent_description}{tools_names}\"\n        tools = component_toolkit(component=self).get_tools(\n            tool_name=\"Call_Agent\", tool_description=description, callbacks=self.get_langchain_callbacks()\n        )\n        if hasattr(self, \"tools_metadata\"):\n            tools = component_toolkit(component=self, metadata=self.tools_metadata).update_tools_metadata(tools=tools)\n        return tools\n"
              },
              "handle_parsing_errors": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "处理解析错误",
                "dynamic": false,
                "info": "智能体是否应在读取用户输入时修复错误以便更好地处理？",
                "list": false,
                "list_add_label": "Add More",
                "name": "handle_parsing_errors",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              },
              "input_value": {
                "_input_type": "MessageTextInput",
                "advanced": false,
                "display_name": "输入",
                "dynamic": false,
                "info": "用户提供的供智能体处理的输入。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "input_value",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": true,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "json_mode": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "JSON 模式",
                "dynamic": false,
                "info": "如果为 True，则无论是否传递模式，都将输出 JSON。",
                "list": false,
                "list_add_label": "Add More",
                "name": "json_mode",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": false
              },
              "max_iterations": {
                "_input_type": "IntInput",
                "advanced": true,
                "display_name": "最大迭代次数",
                "dynamic": false,
                "info": "智能体在停止之前为完成其任务可以进行的最大尝试次数。",
                "list": false,
                "list_add_label": "Add More",
                "name": "max_iterations",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "int",
                "value": 15
              },
              "max_tokens": {
                "_input_type": "IntInput",
                "advanced": true,
                "display_name": "最大令牌数",
                "dynamic": false,
                "info": "要生成的最大令牌数。设置为 0 表示无限令牌。",
                "list": false,
                "list_add_label": "Add More",
                "name": "max_tokens",
                "placeholder": "",
                "range_spec": {
                  "max": 128000,
                  "min": 0,
                  "step": 0.1,
                  "step_type": "float"
                },
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "int",
                "value": ""
              },
              "memory": {
                "_input_type": "HandleInput",
                "advanced": true,
                "display_name": "外部存储器",
                "dynamic": false,
                "info": "从外部存储器检索消息。如果为空，则将使用 Langflow 表。",
                "input_types": [
                  "Memory"
                ],
                "list": false,
                "list_add_label": "Add More",
                "name": "memory",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "trace_as_metadata": true,
                "type": "other",
                "value": ""
              },
              "model_kwargs": {
                "_input_type": "DictInput",
                "advanced": true,
                "display_name": "模型参数",
                "dynamic": false,
                "info": "传递给模型的附加关键字参数。",
                "list": false,
                "list_add_label": "Add More",
                "name": "model_kwargs",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "type": "dict",
                "value": {}
              },
              "model_name": {
                "_input_type": "DropdownInput",
                "advanced": false,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "模型名称",
                "dynamic": false,
                "info": "",
                "load_from_db": false,
                "name": "model_name",
                "options": [
                  "gpt-5-chat",
                  "gpt-4o-mini",
                  "gpt-4o"
                ],
                "options_metadata": [],
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "str",
                "value": "gpt-5-chat"
              },
              "n_messages": {
                "_input_type": "IntInput",
                "advanced": true,
                "display_name": "消息数量",
                "dynamic": false,
                "info": "要检索的消息数量。",
                "list": false,
                "list_add_label": "Add More",
                "name": "n_messages",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "int",
                "value": 100
              },
              "order": {
                "_input_type": "DropdownInput",
                "advanced": true,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "顺序",
                "dynamic": false,
                "info": "消息的顺序。",
                "name": "order",
                "options": [
                  "Ascending",
                  "Descending"
                ],
                "options_metadata": [],
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "Ascending"
              },
              "seed": {
                "_input_type": "IntInput",
                "advanced": true,
                "display_name": "种子",
                "dynamic": false,
                "info": "种子控制作业的可重复性。",
                "list": false,
                "list_add_label": "Add More",
                "name": "seed",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "int",
                "value": 1
              },
              "sender": {
                "_input_type": "DropdownInput",
                "advanced": true,
                "combobox": false,
                "dialog_inputs": {},
                "display_name": "发送者类型",
                "dynamic": false,
                "info": "按发送者类型筛选。",
                "name": "sender",
                "options": [
                  "Machine",
                  "User",
                  "Machine and User"
                ],
                "options_metadata": [],
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "toggle": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "str",
                "value": "Machine and User"
              },
              "sender_name": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "发送者名称",
                "dynamic": false,
                "info": "按发送者名称筛选。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "sender_name",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "session_id": {
                "_input_type": "MessageTextInput",
                "advanced": true,
                "display_name": "会话 ID",
                "dynamic": false,
                "info": "聊天的会话 ID。如果为空，则将使用当前会话 ID 参数。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "session_id",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "system_prompt": {
                "_input_type": "MultilineInput",
                "advanced": false,
                "copy_field": false,
                "display_name": "智能体指令",
                "dynamic": false,
                "info": "系统提示：为指导智能体行为而提供的初始指令和上下文。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "multiline": true,
                "name": "system_prompt",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "###角色设定\n\n您是一位英语面试教练，专为高职高专学生设计。您的风格：\n\n    使用简单、清晰的英语（避免复杂句式和高阶词汇）\n\n    专注于结构化面试问答（常见问题类型：自我简介、优缺点、团队合作、职业规划等）\n\n    不打分、不评分，只提供正面鼓励、内容改进建议和示范回答\n\n    保持耐心、友好，帮助学生建立自信\n\n###核心处理流程\n\n    启动面试\n\n        当用户说“开始面试”、“start interview”、“practice interview”时，您说：\n        “<span style=\"color:blue\">Great! Let’s begin the interview. I’ll ask you a common interview question. Please answer naturally. Here’s the first question: <strong>Can you briefly introduce yourself?</strong>”</span>\n\n        若用户未主动开始，您可询问是否开始练习。\n\n    提问与回答\n\n        您提出一个面试问题\n\n        等待学生回答（学生说完后，您自动进入下一步）\n\n    多轮追问（基于学生回答内容）\n\n        若学生回答太短（<20词，或只说一两句），追问：\n        “<span style=\"color:blue\">Thanks for sharing. Could you tell me a little more? For example, what’s your major or what’s your greatest strength?”</span>\n\n        若学生回答有亮点但不完整（例如提到了技能但没举例），追问：\n        “<span style=\"color:blue\">That’s a good point. Can you give me a specific example from your school or project experience?”</span>\n\n        若学生回答出现明显语法或表达错误，您不打断，继续追问（隐式纠正）：\n        “<span style=\"color:blue\">So, you mean you are hard-working? Could you tell me more about a time when you worked hard to finish a task?”</span>\n\n        每道主问题建议最多2轮追问，之后进入反馈环节。\n\n    反馈与示范（无分数）\n\n        学生完成主问题及追问后，您给出正面反馈 + 可改进点：\n        “<span style=\"color:blue\">Thank you for your answer. I like that you mentioned [某优点]. Here’s a small suggestion to make your answer stronger: [具体改进建议]. Would you like to see a model answer for this question?”</span>\n\n        若用户说“Yes”或“Sure”，您提供示范回答（适合高职高专水平的简单英语，长度60-80词）。\n\n        示范回答后，提供逐句对比（只对比1-2处最明显的改进点，避免过多细节压垮学生）。\n\n    下一题或结束\n\n        完成一题后，询问：\n        “<span style=\"color:blue\">Shall we move to the next question? Or would you like to practice this question again?”</span>\n\n        若用户继续 → 提出下一个面试问题（从题库中按顺序或随机选）\n\n        若用户结束 → “<span style=\"color:blue\">Great job today! Keep practicing these answers. You’re making good progress. See you next time!”</span>\n\n###追问生成指令（动态）\n\n当学生回答后，您自动分析并生成下轮追问：\n\n    长度检测：回答<20词 → 追问“Could you add more details？”\n\n    内容完整性：缺少例子 → 追问“Can you give an example？”\n\n    缺少原因/结果 → 追问“Why was that important?” 或 “What happened next?”\n\n    语法/词汇简单但正确 → 不追问，直接进入反馈\n\n    明显错误（如时态、主谓一致）→ 在追问中自然重述正确形式（不刻意指出错误）\n\n示例：\n学生：“I go to school yesterday.”\n您追问：“Oh, you went to school yesterday? What did you do there?”\n（隐式纠正过去时，不打断交流）\n反馈内容格式（无分数）\n\n反馈应包含三部分：\n\n    正面肯定（至少一句）\n\n    改进建议（最多两条，具体且可操作）\n\n    邀请查看示范回答\n\n输出格式示例：\ntext\n\n<span style=\"color:blue\">Thanks for your answer! I like how you talked about your teamwork experience. That’s very relevant. \nOne small suggestion: you can add a specific result. For example, instead of “I helped my team”, say “I helped my team finish the project two days earlier.” \nWould you like to see a model answer for “Tell me about a time you worked in a team?”</span>\n\n示范回答与逐句比较指令\n\n    示范回答要求：\n\n        长度60-80词，句子简短\n\n        使用常见词汇（B1级）\n\n        结构清晰：观点 → 例子 → 结果\n\n    逐句比较（只比较1-2句）：\n    用表格或列表形式，清晰展示改进点。\n\n示例输出：\ntext\n\n**Model Answer (for \"teamwork\"):**  \nI once worked with two classmates on a class project about online shopping. My role was to collect data. One team member had different ideas at first, but we talked and found a better solution. In the end, we got a good grade and learned to respect each other’s opinions.\n\n**Comparison:**  \nYour sentence: “I worked in a team and we finish the project.”  \nBetter version: “I worked in a team and we finished the project.”  \nWhy change: Use past tense “finished” because the project is done.  \nYour sentence: “It was good.”  \nBetter version: “We got a good grade and learned to respect each other’s opinions.”  \nWhy change: Add a specific result to show success.\n\n比较结束后，询问：\n“<span style=\"color:blue\">Do you have any questions about the model answer? Would you like to try answering the same question again?”</span>\n智能体行为约束\n\n    不使用任何分数、评级、百分数，避免学生感到被评判。\n\n    错误处理：若学生说出“I don’t know”，您回应：\n    “<span style=\"color:blue\">No problem. Let me help you start. For example, you could say… Would you like to try again?”</span>\n\n    多轮对话限制：每道主问题最多3轮（提问 → 学生回答 → 追问一次 → 学生再回答 → 反馈）。避免学生疲劳。\n\n    语言难度：您使用的语言应保持在CEFR A2-B1级别（相当于高职高专英语平均水平）。避免使用诸如“indispensable”、“elaborate”、“nevertheless”等难词。\n\n    鼓励为主：即使学生回答有错误，也先肯定内容再温和地提供修改版。例如：\n    “Great start! Just one small change: instead of ‘I am study’, you can say ‘I study’.”\n\n对话状态控制\n\n    重置：用户说“restart”或“new session” → 清空历史，从自我介绍问题开始。\n\n    跳过：用户说“next question” → 立即换下一个问题，不反馈当前题目。\n\n    重复：用户说“again”或“can you repeat the question” → 原样重复上一问题。\n\n特殊指令（针对高职高专学生）\n\n    部分学生可能不熟悉面试流程。在第一次启动时，您可以主动解释：\n    “<span style=\"color:blue\">Hello! I will act as an interviewer. I’ll ask you common job or school interview questions. You just answer naturally. I won’t give you a score, only friendly advice. Ready? Let’s start: Can you introduce yourself in 3 sentences?”</span>\n\n    若学生回答中使用明显的中式英语（如 “I very like”），您不必直接批评，而是在示范回答中默默使用正确形式（“I really like”）。\n\n    每次反馈后，给学生再次回答同一问题的机会（可选），以强化记忆。"
              },
              "temperature": {
                "_input_type": "SliderInput",
                "advanced": true,
                "display_name": "温度",
                "dynamic": false,
                "info": "",
                "max_label": "",
                "max_label_icon": "",
                "min_label": "",
                "min_label_icon": "",
                "name": "temperature",
                "placeholder": "",
                "range_spec": {
                  "max": 2,
                  "min": 0,
                  "step": 0.01,
                  "step_type": "float"
                },
                "required": false,
                "show": true,
                "slider_buttons": false,
                "slider_buttons_options": [],
                "slider_input": false,
                "title_case": false,
                "tool_mode": false,
                "type": "slider",
                "value": 0.1
              },
              "template": {
                "_input_type": "MultilineInput",
                "advanced": true,
                "copy_field": false,
                "display_name": "模板",
                "dynamic": false,
                "info": "用于格式化数据的模板。它可以包含键 {text}、{sender} 或消息数据中的任何其他键。",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "multiline": true,
                "name": "template",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": "{sender_name}: {text}"
              },
              "tool_calling": {
                "_input_type": "BoolInput",
                "advanced": false,
                "display_name": "Tool Calling",
                "dynamic": false,
                "info": "Enable tool calling capability for the model",
                "list": false,
                "list_add_label": "Add More",
                "name": "tool_calling",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": false
              },
              "tools": {
                "_input_type": "HandleInput",
                "advanced": false,
                "display_name": "工具",
                "dynamic": false,
                "info": "这些是智能体可以用来帮助完成任务的工具。",
                "input_types": [
                  "Tool"
                ],
                "list": true,
                "list_add_label": "Add More",
                "name": "tools",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "trace_as_metadata": true,
                "type": "other",
                "value": ""
              },
              "verbose": {
                "_input_type": "BoolInput",
                "advanced": true,
                "display_name": "详细模式",
                "dynamic": false,
                "info": "",
                "list": false,
                "list_add_label": "Add More",
                "name": "verbose",
                "placeholder": "",
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "bool",
                "value": true
              }
            },
            "tool_mode": false
          },
          "type": "Agent"
        },
        "dragging": false,
        "id": "Agent-Axy3M",
        "measured": {
          "height": 455,
          "width": 320
        },
        "position": {
          "x": 1333.5650219387371,
          "y": 202.71330136860811
        },
        "selected": false,
        "type": "genericNode"
      },
      {
        "data": {
          "id": "AIGCIwriteProcessor-zTx6J",
          "node": {
            "base_classes": [
              "Message"
            ],
            "beta": false,
            "conditional_paths": [],
            "custom_fields": {},
            "description": "输入文本，获取评阅分数数据",
            "display_name": "雅思评阅引擎",
            "documentation": "",
            "edited": false,
            "field_order": [
              "content"
            ],
            "frozen": false,
            "icon": "Json",
            "legacy": false,
            "lf_version": "",
            "metadata": {},
            "minimized": false,
            "output_types": [],
            "outputs": [
              {
                "allows_loop": false,
                "cache": true,
                "display_name": "Toolset",
                "group_outputs": false,
                "hidden": null,
                "method": "to_toolkit",
                "name": "component_as_tool",
                "options": null,
                "required_inputs": null,
                "selected": "Tool",
                "tool_mode": true,
                "types": [
                  "Tool"
                ],
                "value": "__UNDEFINED__"
              }
            ],
            "pinned": false,
            "template": {
              "_type": "Component",
              "code": {
                "advanced": true,
                "dynamic": true,
                "fileTypes": [],
                "file_path": "",
                "info": "",
                "list": false,
                "load_from_db": false,
                "multiline": true,
                "name": "code",
                "password": false,
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "type": "code",
                "value": "import json\nimport requests\nimport os\n\nfrom langflow.custom import Component\nfrom langflow.io import MessageTextInput, Output\nfrom langflow.schema.message import Message\n\n\nclass AIGCIwriteProcessorComponent(Component):\n    \"\"\"接收文本内容并将其通过API处理为JSON格式的组件\"\"\"\n\n    display_name = \"雅思评阅引擎\"\n    description = \"输入文本，获取评阅分数数据\"\n    icon = \"Json\"\n    name = \"AIGCIwriteProcessor\"\n    api_url = os.environ.get(\"AIGC_URL\", \"https://aigc.unipus.cn\") + \"/api/lf/iwrite/icorrect\"\n    inputs = [\n        MessageTextInput(\n            name=\"content\",\n            display_name=\"内容\",\n            info=\"要处理的文本内容\",\n            required=True,\n        )\n    ]\n\n    outputs = [\n        Output(display_name=\"JSON结果\", name=\"json_result\", method=\"process_content\"),\n    ]\n\n    async def process_content(self) -> Message:\n        \"\"\"处理内容并返回JSON结果\"\"\"\n        token = await self.get_variables(\"_aigc_token\", \"Token\")\n        if not self.content:\n            self.status = \"未提供内容\"\n            return Message(text=\"\")\n\n        try:\n            # 准备API请求参数\n            params = {\n                \"content\": self.content\n            }\n            \n            # 准备请求头\n            headers = {\n                \"Content-Type\": \"application/json\",\n                \"User-Agent\": \"Langflow/1.3.1\",\n                \"Accept\": \"application/json\",\n                \"token\": token\n            }\n            \n            # 发送请求到API\n            response = requests.post(self.api_url, json=params, headers=headers)\n            response.raise_for_status()  # 如果请求失败则引发异常\n            \n            # 解析响应\n            result = response.json()\n            \n            # 将结果转换为格式化的JSON文本\n            formatted_json = json.dumps(result, ensure_ascii=False, indent=2)\n            \n            # 更新状态并返回结果\n            self.status = f\"成功处理 {len(self.content)} 字符的内容\"\n            return Message(text=formatted_json)\n            \n        except requests.exceptions.RequestException as e:\n            error_message = f\"API请求错误: {str(e)}\"\n            self.status = error_message\n            return Message(text=error_message)\n        \n        except json.JSONDecodeError as e:\n            error_message = f\"JSON解析错误: {str(e)}\"\n            self.status = error_message\n            return Message(text=error_message)\n        \n        except Exception as e:\n            error_message = f\"处理内容时出错: {str(e)}\"\n            self.status = error_message\n            return Message(text=error_message) "
              },
              "content": {
                "_input_type": "MessageTextInput",
                "advanced": false,
                "display_name": "内容",
                "dynamic": false,
                "info": "要处理的文本内容",
                "input_types": [
                  "Message"
                ],
                "list": false,
                "list_add_label": "Add More",
                "load_from_db": false,
                "name": "content",
                "placeholder": "",
                "required": true,
                "show": true,
                "title_case": false,
                "tool_mode": true,
                "trace_as_input": true,
                "trace_as_metadata": true,
                "type": "str",
                "value": ""
              },
              "tools_metadata": {
                "_input_type": "ToolsInput",
                "advanced": false,
                "display_name": "Actions",
                "dynamic": false,
                "info": "Modify tool names and descriptions to help agents understand when to use each tool.",
                "is_list": true,
                "list_add_label": "Add More",
                "name": "tools_metadata",
                "placeholder": "",
                "real_time_refresh": true,
                "required": false,
                "show": true,
                "title_case": false,
                "tool_mode": false,
                "trace_as_metadata": true,
                "type": "tools",
                "value": [
                  {
                    "args": {
                      "content": {
                        "description": "要处理的文本内容",
                        "title": "Content",
                        "type": "string"
                      }
                    },
                    "description": "AIGCIwriteProcessor. process_content - 输入文本，获取评阅分数数据",
                    "display_description": "AIGCIwriteProcessor. process_content - 输入文本，获取评阅分数数据",
                    "display_name": "process_content",
                    "name": "process_content",
                    "readonly": false,
                    "status": true,
                    "tags": [
                      "process_content"
                    ]
                  }
                ]
              }
            },
            "tool_mode": true
          },
          "showNode": true,
          "type": "AIGCIwriteProcessor"
        },
        "dragging": false,
        "id": "AIGCIwriteProcessor-zTx6J",
        "measured": {
          "height": 201,
          "width": 320
        },
        "position": {
          "x": 935.2231634766142,
          "y": 85.8844798749269
        },
        "selected": false,
        "type": "genericNode"
      }
    ],
    "viewport": {
      "x": -477.90993011999035,
      "y": -35.326837734944775,
      "zoom": 0.7013598816894148
    }
  },
  "description": "英语结构化面试口语训练智能体",
  "endpoint_name": null,
  "id": "759a3d4d-6977-4c36-b6ed-311c212ffd79",
  "is_component": false,
  "last_tested_version": "",
  "name": "英语口语面试智能体",
  "tags": []
}

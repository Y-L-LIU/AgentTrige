## PDFTriage: Question Answering over Long, Structured Documents

# PDFtriage

PDFtriage: 用于结构化文档问答的新方法，提供了基于结构和内容的上下文检索，解决了现有模型在处理结构化文档时的局限性

## Dependencies

- llama-index==0.8.56

## Usage

1. **Scan and Parse PDF Files**

   Use adobe PDFExtract
2. **Set Environment Variables**

   在使用 PDFtriage 之前，你需要设置一些环境变量。你可以在 .env.example 文件中找到示例，并按照相同的格式创建一个 .env 文件。以下是需要设置的环境变量：

   ```plaintext
   OPENAI_API_KEY=Your_OpenAI_API_Key
   OPENAI_API_BASE=API_Base_URL
   FILE_PATH=Path_to_the_JSON_Data_File_of_the_Parsed_PDF
3. use `src_new/inspect_json` to get the tree file with the PDFExtract output
4. Play with tree search
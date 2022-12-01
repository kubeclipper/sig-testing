1. 安装pandoc
https://pandoc.org/installing.html

2. 生成word
find . -name "*.md" | sort | xargs pandoc -s --reference-doc reference.docx -o ./testcases.docx

3. 生成html
find . -name "*.md" | sort | xargs pandoc -s --toc --template=template.html --metadata pagetitle='测试用例' -o ./testcases.html

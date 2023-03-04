# NICAR23 Money

Uncovering Underground Money Networks: A Deep Dive into Investigative Journalism Techniques and Tools.

## List of Resources

[Aleph](https://github.com/alephdata/aleph) - A tool for managing large collections of documents and extracting structured data from them.

[OCCRP catalog of research databases](https://id.occrp.org/databases/) - Global index of public registries for company, land and court records. OCCRP has pulled together over 1,000 sources from 181 countries.

[DomainTools](https://www.domaintools.com/) - Historical WHOIS information and domain name registration data. Recently purchased Farsight Security, which has a lot of DNS data.

## Example code

### Summarize long documents using AI

[summarizer.py](nicar23_money/summarizer.py)

Example code that loads a language model and uses it, along with other packages, to extract text from a PDF, split it into chunks, and summarize it using a "map reduce" summarization chain from the langchain library. It then prints the summary.

To run, first install the requirements. If you use `Poetry`, you can do this with `poetry install`. Otherwise, you can use `pip install -r requirements.txt`.

Then copy .env.example to .env and fill in the values for the OpenAI API key, which you can get from [here](https://platform.openai.com/).

Then, run the script with:

```bash
python -m nicar23_money.summarizer <filename>
```

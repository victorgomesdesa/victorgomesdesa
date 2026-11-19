[Português (Brasil)](./README.pt-BR.md)

![A black cat watches a document land in a tray on a CRT monitor.](./assets/banner.png)

# Victor Gomes de Sá

I build web apps and automate business workflows. When I build a form, I want to know what happens to the data if someone clicks the same button twice.

### Invoicing and inventory

In this coding challenge, I split billing and inventory into two Go services behind an Angular app. One tricky case was an invoice that stayed open after inventory had already deducted the stock. I gave each closing operation its own key so billing could retry after a lost response without deducting the same items twice.

[Source code](https://github.com/victorgomesdesa/Korp_Teste_VictorGomesDeSa) · [Architecture notes](https://github.com/victorgomesdesa/Korp_Teste_VictorGomesDeSa/blob/main/docs/technical-design.md)

### Team evaluations

I built a React and FastAPI app where managers can evaluate people in their reporting chain. Two managers can evaluate the same person in a given week, but each can submit only once. A PostgreSQL constraint enforces that rule even when two requests arrive together.

[Source code](https://github.com/victorgomesdesa/employee-evaluation-platform) · [Weekly limit tests](https://github.com/victorgomesdesa/employee-evaluation-platform/blob/1e1a926f3eedcc451051f50ce4823cfb3d64c882/backend/tests/test_evaluation_submission.py#L208-L240) · [Concurrent submissions test](https://github.com/victorgomesdesa/employee-evaluation-platform/blob/1e1a926f3eedcc451051f50ce4823cfb3d64c882/backend/tests/test_evaluation_submission.py#L495)

### Automation at work

I brought several bots' run results into one place so the team could check on them together. In a separate tool for tax documents, I added a way to resume interrupted requests.

My portfolio has a playable arcade. You can also click the cat and ask it about my work. [Visit my portfolio](https://victorgomesdesa.github.io/)

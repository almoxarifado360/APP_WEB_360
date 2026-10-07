ESTOQUE 360 — Atualização do Inventário por Arquivo

Arquivos:
- index.html: nova importação de inventário por PDF, PNG, JPEG, Excel e Word (.docx), mantendo conferência antes da gravação.
- API_APP_360_V26_INVENTARIO_ARQUIVO.gs: backend com data individual por item de inventário.
- sw.js: cache atualizado para v20.
- manifest.json: mantido.

Fluxo:
1. Selecionar/importar arquivo.
2. O app lê código + quantidade.
3. Os itens aparecem em “Materiais em conferência”.
4. O usuário revisa/edita a contagem.
5. Só em “FINALIZAR INVENTÁRIO” o ESTOQUE é alterado.
6. G = Contagem de inventário; H = Data do inventário; I = Estoque atual.
7. A data usada em cada item é a data/hora em que ele foi importado/adicionado.

Bibliotecas externas carregadas pelo index.html:
- SheetJS (Excel)
- PDF.js (PDF)
- Mammoth.js (Word .docx)
- Tesseract.js (OCR de imagens/PDFs escaneados)

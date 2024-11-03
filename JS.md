# JS

```javascript
function insertMarkdown(text) {
            const textarea = document.getElementById('content');
            const start = textarea.selectionStart;
            const end = textarea.selectionEnd;
            // Insert the markdown text at the cursor position
            textarea.value = textarea.value.substring(0, start) + text + textarea.value.substring(end);
            // Move the cursor to the end of the inserted text
            textarea.selectionStart = textarea.selectionEnd = start + text.length;
            textarea.focus();
        }
```

---

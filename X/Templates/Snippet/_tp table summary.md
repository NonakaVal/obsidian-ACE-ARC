>[!SUMMARY]- Table of Contents
<%*
    let headers = await tp.file.content
        .split('\n') // split file into lines
        .filter(t => t.match(/^[#]+\s+/gi)) // only get headers
        .map(h => {
            let header_level = h.split(' ')[0].match(/#/g).length;
             // get header text without special characters like '[' and ']'
            let header_text = h.substring(h.indexOf(' ') + 1).replace(/[\[\]]+/g, '');
            let header_link = `[[${tp.file.title}#${header_text}|${header_text}]]`

            // prepend block-quote (>), indentation and bullet-point (-)
            return `>${'    '.repeat(header_level - 1) + '- ' + header_link}`;
        })
        .join('\n')
%><% headers %>
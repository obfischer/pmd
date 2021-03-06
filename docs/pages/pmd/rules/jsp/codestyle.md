---
title: Codestyle
summary: Rules which enforce a specific coding style.
permalink: pmd_rules_jsp_codestyle.html
folder: pmd/rules/jsp
sidebaractiveurl: /pmd_rules_jsp.html
editmepath: ../pmd-jsp/src/main/resources/category/jsp/codestyle.xml
keywords: Codestyle, DuplicateJspImports
---
## DuplicateJspImports

**Since:** PMD 3.7

**Priority:** Medium (3)

Avoid duplicate import statements inside JSP's.

**This rule is defined by the following Java class:** [net.sourceforge.pmd.lang.jsp.rule.codestyle.DuplicateJspImportsRule](https://github.com/pmd/pmd/blob/master/pmd-jsp/src/main/java/net/sourceforge/pmd/lang/jsp/rule/codestyle/DuplicateJspImportsRule.java)

**Example(s):**

``` jsp
<%@ page import=\"com.foo.MyClass,com.foo.MyClass\"%><html><body><b><img src=\"<%=Some.get()%>/foo\">xx</img>text</b></body></html>
```

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/jsp/codestyle.xml/DuplicateJspImports" />
```


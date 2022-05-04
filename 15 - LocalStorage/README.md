1-<label> for
即和 <label> 元素在同一文档中的 可关联标签的元素 的 id。 文档中第一个 id 值与 <label> 元素 for 属性值相同的元素，如果可关联标签（labelable），则为已关联标签的控件，其标签就是这个 <label> 元素。如果这个元素不可关联标签，则 for 属性没有效果。如果文档中还有其他元素的 id 值也和 for 属性相同，for 属性对这些元素也没有影响

  
2- Attribute selector
  
Selects all elements that have the given attribute. Syntax: [attr] [attr=value] [attr~=value] [attr|=value] [attr^=value] [attr$=value] [attr*=value] Example: [autoplay] will match all elements that have the autoplay attribute set (to any value).
3-Behaviour delegation:
  
  

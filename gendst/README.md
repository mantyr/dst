Lists:
```
Field.Names:        []*Ident ","
FieldList.List:     []*Field "\n" or ";"
CompositeLit.Elts:  []Expr   ","
CallExpr.Args:      []Expr   ","
AssignStmt.Lhs:     []Expr   ","
AssignStmt.Rhs:     []Expr   ","
ReturnStmt.Results: []Expr   ","
BlockStmt.List:     []Stmt   "\n" or ";"
CaseClause:List:    []Expr   ","
CaseClause.Body:    []Stmt   "\n" or ";"
CommClause.Body:    []Stmt   "\n" or ";"
ValueSpec.Names:    []*Ident ","
ValueSpec.Values:   []Expr   ","
GenDecl.Specs:      []Spec   "\n" or ";"
File.Decls:         []Decl   "\n" or ";"
File.Imports:       []*ImportSpec "\n" or ";"?
```


Fragments:
```
Opening [FieldList(Pos)]
Closing [FieldList(Pos)]
For [ForStmt(Pos) RangeStmt(Pos)]
Key [KeyValueExpr(Node) MapType(Node) RangeStmt(Node)]
Select [SelectStmt(Pos)]
Switch [SwitchStmt(Pos) TypeSwitchStmt(Pos)]
Rparen [CallExpr(Pos) GenDecl(Pos) ParenExpr(Pos) TypeAssertExpr(Pos)]
Lparen [CallExpr(Pos) GenDecl(Pos) ParenExpr(Pos) TypeAssertExpr(Pos)]
Rbrack [IndexExpr(Pos) SliceExpr(Pos)]
Lbrack [ArrayType(Pos) IndexExpr(Pos) SliceExpr(Pos)]
Rbrace [BlockStmt(Pos) CompositeLit(Pos)]
Lbrace [BlockStmt(Pos) CompositeLit(Pos)]
Text [Comment(string)]
Type [CompositeLit(Node) Field(Node) FuncDecl(Node) FuncLit(Node) TypeAssertExpr(Node) TypeSpec(Node) ValueSpec(Node)]
Call [DeferStmt(Node) GoStmt(Node)]
Index [IndexExpr(Node)]
Fields [StructType(Node)]
Tok [AssignStmt(Token) BranchStmt(Token) GenDecl(Token) IncDecStmt(Token) RangeStmt(Token)]
Op [BinaryExpr(Token) UnaryExpr(Token)]
Slash [Comment(Pos)]
Decls [File([]Node)]
Post [ForStmt(Node)]
Func [FuncType(Pos)]
Len [ArrayType(Node)]
Y [BinaryExpr(Node)]
Elts [CompositeLit([]Node)]
Path [ImportSpec(Node)]
Interface [InterfaceType(Pos)]
Return [ReturnStmt(Pos)]
Begin [ChanType(Pos)]
Sel [SelectorExpr(Node)]
Assign [TypeSpec(Pos) TypeSwitchStmt(Node)]
Value [BasicLit(string) ChanType(Node) KeyValueExpr(Node) MapType(Node) RangeStmt(Node) SendStmt(Node)]
List [BlockStmt([]Node) CaseClause([]Node) CommentGroup([]Node) FieldList([]Node)]
Body [CaseClause([]Node) CommClause([]Node) ForStmt(Node) FuncDecl(Node) FuncLit(Node) IfStmt(Node) RangeStmt(Node) SelectStmt(Node) SwitchStmt(Node) TypeSwitchStmt(Node)]
Name [File(Node) FuncDecl(Node) Ident(string) ImportSpec(Node) TypeSpec(Node)]
Chan [SendStmt(Node)]
Max [SliceExpr(Node)]
Elt [ArrayType(Node) Ellipsis(Node)]
Args [CallExpr([]Node)]
Doc [Field(Node) File(Node) FuncDecl(Node) GenDecl(Node) ImportSpec(Node) TypeSpec(Node) ValueSpec(Node)]
Methods [InterfaceType(Node)]
Map [MapType(Pos)]
Label [BranchStmt(Node) LabeledStmt(Node)]
Arrow [ChanType(Pos) SendStmt(Pos)]
Tag [Field(Node) SwitchStmt(Node)]
Results [FuncType(Node) ReturnStmt([]Node)]
Init [ForStmt(Node) IfStmt(Node) SwitchStmt(Node) TypeSwitchStmt(Node)]
Fun [CallExpr(Node)]
Colon [CaseClause(Pos) CommClause(Pos) KeyValueExpr(Pos) LabeledStmt(Pos)]
Comm [CommClause(Node)]
Values [ValueSpec([]Node)]
Low [SliceExpr(Node)]
High [SliceExpr(Node)]
Lhs [AssignStmt([]Node)]
Names [Field([]Node) ValueSpec([]Node)]
Package [File(Pos)]
Case [CaseClause(Pos) CommClause(Pos)]
Semicolon [EmptyStmt(Pos)]
If [IfStmt(Pos)]
Defer [DeferStmt(Pos)]
Specs [GenDecl([]Node)]
Params [FuncType(Node)]
Struct [StructType(Pos)]
Ellipsis [CallExpr(Pos) Ellipsis(Pos)]
Cond [ForStmt(Node) IfStmt(Node)]
Go [GoStmt(Pos)]
Else [IfStmt(Node)]
X [BinaryExpr(Node) ExprStmt(Node) IncDecStmt(Node) IndexExpr(Node) ParenExpr(Node) RangeStmt(Node) SelectorExpr(Node) SliceExpr(Node) StarExpr(Node) TypeAssertExpr(Node) UnaryExpr(Node)]
Decl [DeclStmt(Node)]
Comment [Field(Node) ImportSpec(Node) TypeSpec(Node) ValueSpec(Node)]
Recv [FuncDecl(Node)]
Rhs [AssignStmt([]Node)]
Stmt [LabeledStmt(Node)]
Star [StarExpr(Pos)]
```

Node start:
```
From [BadDecl(Pos) BadExpr(Pos) BadStmt(Pos)]
```

Node end:
```
To [BadDecl(Pos) BadExpr(Pos) BadStmt(Pos)]
EndPos [ImportSpec(Pos)]
```

Special:
```
Dir [ChanType(ChanDir)]
Unresolved [File([]Node)]
Obj [Ident(Object)]
Comments [File([]Node)]
Implicit [EmptyStmt(bool)]
Kind [BasicLit(Token)]
Incomplete [CompositeLit(bool) InterfaceType(bool) StructType(bool)]
Scope [File(Scope)]
Imports [File([]Node)]
Slice3 [SliceExpr(bool)]
```

Fragment position:
```
ValuePos [BasicLit(Pos)]
TokPos [AssignStmt(Pos) BranchStmt(Pos) GenDecl(Pos) IncDecStmt(Pos) RangeStmt(Pos)]
NamePos [Ident(Pos)]
OpPos [BinaryExpr(Pos) UnaryExpr(Pos)]
```

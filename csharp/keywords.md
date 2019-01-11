# Keywords

- Keywords: reserved and contextual.
- Reserved keywords can be used as user identifiers only if prefixed by `@`
- The symbol `@` doesn't count as part of identifier.


Keywords are predefined, reserved identifiers that have special meanings to the compiler. They cannot be used as identifiers in your program unless they include `@` as a prefix, e.g. `@if` is a valid identifier. The `@` symbol doesn't form a part of the identifier itself, e.g. `@id` is the same identifier as `id`.

The contextual keywords have special meaning only in a limited program context and can be used as identifiers outside that context. Some contextual keywords, such as `partial` and `where`, have special meanings in two or more contexts. Generally, new keywords are added as contextual keywords, for backwards compatibility.



## Reserved keywords

```
private
protected
public
internal
readonly
abstract
as
is
bool
char
byte
sbyte
double
long
decimal
float
true
int
string
false
break
continue
try
switch
case
if
for
foreach
goto
do
else
throw
catch
finally
namespace
class
struct
enum
delegate
event
interface
default
const
extern
fixed
explicit
implicit
base
this
in
lock
new
null
object
operator
out
override
params
ref
return
short
sizeof
stackalloc
sealed
static
checked
unchecked
```



## Contextual keywords

```
ascending
descending
async
await
var
nameof
dynamic
by
equals
from
get
global
add
select
group
orderby
when
where
join
in
into
let
on
partial
remove
set
value
yield
```




## Reserved Keywords: alphabetical horizotal

| 1        | 2        | 3         | 4            | 5         |
|----------|----------|-----------|--------------|-----------|
| abstract | do       | in        | protected    | throw     |
| as       | double   | int       | public       | true      |
| base     | else     | interface | readonly     | try       |
| bool     | enum     | internal  | ref          | typeof    |
| break    | event    | is        | return       | uint      |
| byte     | explicit | lock      | sbyte        | ulong     |
| case     | extern   | long      | sealed       | unchecked |
| catch    | false    | namespace | short        | unsafe    |
| char     | finally  | new       | sizeof       | ushort    |
| checked  | fixed    | null      | stackalloc   | using     |
| class    | float    | object    | static       | virtual   |
| const    | for      | operator  | using static | void      |
| continue | foreach  | out       | string       | volatile  |
| decimal  | goto     | override  | struct       | while     |
| default  | if       | params    | switch       |           |
| delegate | implicit | private   | this         |           |



## Reserved Keywords: alphabetical vertical

| 1        | 2        | 3          | 4            | 5         |
|----------|----------|------------|--------------|-----------|
| abstract | as       | base       | bool         | break     |
| byte     | case     | catch      | char         | checked   |
| class    | const    | continue   | decimal      | default   |
| delegate | do       | double     | else         | enum      |
| event    | explicit | extern     | false        | finally   |
| fixed    | float    | for        | foreach      | goto      |
| if       | implicit | in         | int          | interface |
| internal | is       | lock       | long         | namespace |
| new      | null     | object     | operator     | out       |
| override | params   | private    | protected    | public    |
| readonly | ref      | return     | sbyte        | sealed    |
| short    | sizeof   | stackalloc | static       | string    |
| struct   | switch   | this       | throw        | true      |
| try      | typeof   | uint       | ulong        | unchecked |
| unsafe   | ushort   | using      | using static | virtual   |
| void     | volatile | while      |              |           |


## Contextual Keywords: alphabetical


```
add   alias   ascending
async   await   by
descending   dynamic   equals
from   get   global
group   into   join
let   nameof   on
orderby   partial (type)   partial (method)
remove   select   set
value   var   when (filter condition)
where (generic type constraint)   where (query clause)   yield
```

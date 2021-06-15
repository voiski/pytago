# pythagoras

Transpiles some Python into human-readable Golang.

## Support

- No X means no support as of yet. 
- Decent+ means there's at least extensive support, and I may not have thought of a way it could break yet. 
- Limited means there's at least some facet of programming in place that deals with this (either explicitly or implicitly),
 although there may be serious limitations. Check the notes for more.

|Support                       |Decent+|Limited|Notes                                                                                          |Category                                     |
|------------------------------|-------|-------|-----------------------------------------------------------------------------------------------|---------------------------------------------|
|False                         |X      |       |                                                                                               |Keywords                                     |
|None                          |X      |       |                                                                                               |Keywords                                     |
|True                          |X      |       |                                                                                               |Keywords                                     |
|and                           |X      |       |                                                                                               |Keywords                                     |
|as                            |X      |       |                                                                                               |Keywords                                     |
|assert                        |       |       |                                                                                               |Keywords                                     |
|async                         |       |       |                                                                                               |Keywords                                     |
|await                         |       |       |                                                                                               |Keywords                                     |
|break                         |X      |       |                                                                                               |Keywords                                     |
|class                         |       |       |                                                                                               |Keywords                                     |
|continue                      |X      |       |                                                                                               |Keywords                                     |
|def                           |       |X      |Limited type inference                                                                         |Keywords                                     |
|del                           |X      |       |                                                                                               |Keywords                                     |
|elif                          |X      |       |                                                                                               |Keywords                                     |
|else                          |X      |       |                                                                                               |Keywords                                     |
|except                        |       |       |                                                                                               |Keywords                                     |
|finally                       |       |       |                                                                                               |Keywords                                     |
|for                           |       |X      |No list comprehension / unpacking support.                                                     |Keywords                                     |
|from                          |X      |       |                                                                                               |Keywords                                     |
|global                        |       |       |                                                                                               |Keywords                                     |
|if                            |       |X      |Newly declared variables will not be available outside.                                        |Keywords                                     |
|import                        |X      |       |                                                                                               |Keywords                                     |
|in                            |       |       |                                                                                               |Keywords                                     |
|is                            |       |       |                                                                                               |Keywords                                     |
|lambda                        |       |X      |Limited type inference                                                                         |Keywords                                     |
|nonlocal                      |       |       |                                                                                               |Keywords                                     |
|not                           |X      |       |                                                                                               |Keywords                                     |
|or                            |X      |       |                                                                                               |Keywords                                     |
|pass                          |X      |       |                                                                                               |Keywords                                     |
|raise                         |       |       |                                                                                               |Keywords                                     |
|return                        |X      |       |                                                                                               |Keywords                                     |
|try                           |       |       |                                                                                               |Keywords                                     |
|while                         |       |X      |Newly declared variables will not be available outside.                                        |Keywords                                     |
|with                          |X      |       |                                                                                               |Keywords                                     |
|yield                         |       |       |                                                                                               |Keywords                                     |
|ArithmeticError               |       |       |                                                                                               |Built-ins                                    |
|AssertionError                |       |       |                                                                                               |Built-ins                                    |
|AttributeError                |       |       |                                                                                               |Built-ins                                    |
|BaseException                 |       |       |                                                                                               |Built-ins                                    |
|BlockingIOError               |       |       |                                                                                               |Built-ins                                    |
|BrokenPipeError               |       |       |                                                                                               |Built-ins                                    |
|BufferError                   |       |       |                                                                                               |Built-ins                                    |
|BytesWarning                  |       |       |                                                                                               |Built-ins                                    |
|ChildProcessError             |       |       |                                                                                               |Built-ins                                    |
|ConnectionAbortedError        |       |       |                                                                                               |Built-ins                                    |
|ConnectionError               |       |       |                                                                                               |Built-ins                                    |
|ConnectionRefusedError        |       |       |                                                                                               |Built-ins                                    |
|ConnectionResetError          |       |       |                                                                                               |Built-ins                                    |
|DeprecationWarning            |       |       |                                                                                               |Built-ins                                    |
|EOFError                      |       |       |                                                                                               |Built-ins                                    |
|Ellipsis                      |       |X      |Treated like a pass                                                                            |Built-ins                                    |
|EncodingWarning               |       |       |                                                                                               |Built-ins                                    |
|EnvironmentError              |       |       |                                                                                               |Built-ins                                    |
|Exception                     |       |       |                                                                                               |Built-ins                                    |
|FileExistsError               |       |       |                                                                                               |Built-ins                                    |
|FileNotFoundError             |       |       |                                                                                               |Built-ins                                    |
|FloatingPointError            |       |       |                                                                                               |Built-ins                                    |
|FutureWarning                 |       |       |                                                                                               |Built-ins                                    |
|GeneratorExit                 |       |       |                                                                                               |Built-ins                                    |
|IOError                       |       |       |                                                                                               |Built-ins                                    |
|ImportError                   |       |       |                                                                                               |Built-ins                                    |
|ImportWarning                 |       |       |                                                                                               |Built-ins                                    |
|IndentationError              |       |       |                                                                                               |Built-ins                                    |
|IndexError                    |       |       |                                                                                               |Built-ins                                    |
|InterruptedError              |       |       |                                                                                               |Built-ins                                    |
|IsADirectoryError             |       |       |                                                                                               |Built-ins                                    |
|KeyError                      |       |       |                                                                                               |Built-ins                                    |
|KeyboardInterrupt             |       |       |                                                                                               |Built-ins                                    |
|LookupError                   |       |       |                                                                                               |Built-ins                                    |
|MemoryError                   |       |       |                                                                                               |Built-ins                                    |
|ModuleNotFoundError           |       |       |                                                                                               |Built-ins                                    |
|NameError                     |       |       |                                                                                               |Built-ins                                    |
|NotADirectoryError            |       |       |                                                                                               |Built-ins                                    |
|NotImplemented                |       |       |                                                                                               |Built-ins                                    |
|NotImplementedError           |       |       |                                                                                               |Built-ins                                    |
|OSError                       |       |       |                                                                                               |Built-ins                                    |
|OverflowError                 |       |       |                                                                                               |Built-ins                                    |
|PendingDeprecationWarning     |       |       |                                                                                               |Built-ins                                    |
|PermissionError               |       |       |                                                                                               |Built-ins                                    |
|ProcessLookupError            |       |       |                                                                                               |Built-ins                                    |
|RecursionError                |       |       |                                                                                               |Built-ins                                    |
|ReferenceError                |       |       |                                                                                               |Built-ins                                    |
|ResourceWarning               |       |       |                                                                                               |Built-ins                                    |
|RuntimeError                  |       |       |                                                                                               |Built-ins                                    |
|RuntimeWarning                |       |       |                                                                                               |Built-ins                                    |
|StopAsyncIteration            |       |       |                                                                                               |Built-ins                                    |
|StopIteration                 |       |       |                                                                                               |Built-ins                                    |
|SyntaxError                   |       |       |                                                                                               |Built-ins                                    |
|SyntaxWarning                 |       |       |                                                                                               |Built-ins                                    |
|SystemError                   |       |       |                                                                                               |Built-ins                                    |
|SystemExit                    |       |       |                                                                                               |Built-ins                                    |
|TabError                      |       |       |                                                                                               |Built-ins                                    |
|TimeoutError                  |       |       |                                                                                               |Built-ins                                    |
|TypeError                     |       |       |                                                                                               |Built-ins                                    |
|UnboundLocalError             |       |       |                                                                                               |Built-ins                                    |
|UnicodeDecodeError            |       |       |                                                                                               |Built-ins                                    |
|UnicodeEncodeError            |       |       |                                                                                               |Built-ins                                    |
|UnicodeError                  |       |       |                                                                                               |Built-ins                                    |
|UnicodeTranslateError         |       |       |                                                                                               |Built-ins                                    |
|UnicodeWarning                |       |       |                                                                                               |Built-ins                                    |
|UserWarning                   |       |       |                                                                                               |Built-ins                                    |
|ValueError                    |       |       |                                                                                               |Built-ins                                    |
|Warning                       |       |       |                                                                                               |Built-ins                                    |
|WindowsError                  |       |       |                                                                                               |Built-ins                                    |
|ZeroDivisionError             |       |       |                                                                                               |Built-ins                                    |
|_                             |       |       |                                                                                               |Built-ins                                    |
|__build_class__               |       |       |                                                                                               |Built-ins                                    |
|__debug__                     |       |       |                                                                                               |Built-ins                                    |
|__doc__                       |       |       |                                                                                               |Built-ins                                    |
|__import__                    |       |       |                                                                                               |Built-ins                                    |
|__loader__                    |       |       |                                                                                               |Built-ins                                    |
|__name__                      |       |       |                                                                                               |Built-ins                                    |
|__package__                   |       |       |                                                                                               |Built-ins                                    |
|__spec__                      |       |       |                                                                                               |Built-ins                                    |
|abs                           |       |       |                                                                                               |Built-ins                                    |
|aiter                         |       |       |                                                                                               |Built-ins                                    |
|all                           |       |       |                                                                                               |Built-ins                                    |
|anext                         |       |       |                                                                                               |Built-ins                                    |
|any                           |       |       |                                                                                               |Built-ins                                    |
|ascii                         |       |       |                                                                                               |Built-ins                                    |
|bin                           |       |       |                                                                                               |Built-ins                                    |
|bool                          |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|breakpoint                    |       |       |                                                                                               |Built-ins                                    |
|bytearray                     |       |       |                                                                                               |Built-ins                                    |
|bytes                         |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|callable                      |       |       |                                                                                               |Built-ins                                    |
|chr                           |       |       |                                                                                               |Built-ins                                    |
|classmethod                   |       |       |                                                                                               |Built-ins                                    |
|compile                       |       |       |                                                                                               |Built-ins                                    |
|complex                       |       |       |                                                                                               |Built-ins                                    |
|copyright                     |       |       |                                                                                               |Built-ins                                    |
|credits                       |       |       |                                                                                               |Built-ins                                    |
|delattr                       |       |       |                                                                                               |Built-ins                                    |
|dict                          |       |       |                                                                                               |Built-ins                                    |
|dir                           |       |       |                                                                                               |Built-ins                                    |
|divmod                        |       |       |                                                                                               |Built-ins                                    |
|enumerate                     |       |       |Looping over an enumerate produces a go range loop.                                            |Built-ins                                    |
|eval                          |       |       |                                                                                               |Built-ins                                    |
|exec                          |       |       |                                                                                               |Built-ins                                    |
|exit                          |       |       |                                                                                               |Built-ins                                    |
|filter                        |       |       |                                                                                               |Built-ins                                    |
|float                         |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|format                        |       |       |                                                                                               |Built-ins                                    |
|frozenset                     |       |       |                                                                                               |Built-ins                                    |
|getattr                       |       |       |                                                                                               |Built-ins                                    |
|globals                       |       |       |                                                                                               |Built-ins                                    |
|hasattr                       |       |       |                                                                                               |Built-ins                                    |
|hash                          |       |       |                                                                                               |Built-ins                                    |
|help                          |       |       |                                                                                               |Built-ins                                    |
|hex                           |       |       |                                                                                               |Built-ins                                    |
|id                            |       |       |                                                                                               |Built-ins                                    |
|input                         |       |       |                                                                                               |Built-ins                                    |
|int                           |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|isinstance                    |       |       |                                                                                               |Built-ins                                    |
|issubclass                    |       |       |                                                                                               |Built-ins                                    |
|iter                          |       |       |                                                                                               |Built-ins                                    |
|len                           |       |X      |Incidentally, len in Go is similar to len in Python. YMMV.                                     |Built-ins                                    |
|license                       |       |       |                                                                                               |Built-ins                                    |
|list                          |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|locals                        |       |       |                                                                                               |Built-ins                                    |
|map                           |       |       |                                                                                               |Built-ins                                    |
|max                           |       |       |                                                                                               |Built-ins                                    |
|memoryview                    |       |       |                                                                                               |Built-ins                                    |
|min                           |       |       |                                                                                               |Built-ins                                    |
|next                          |       |       |                                                                                               |Built-ins                                    |
|object                        |       |       |                                                                                               |Built-ins                                    |
|oct                           |       |       |                                                                                               |Built-ins                                    |
|open                          |       |X      |Opening files supported with all modes.                                                        |Built-ins                                    |
|ord                           |       |       |                                                                                               |Built-ins                                    |
|pow                           |       |       |                                                                                               |Built-ins                                    |
|print                         |       |X      |Print calls replaced with calls to fmt.println. No kw support. Multi-argument support untested.|Built-ins                                    |
|property                      |       |       |                                                                                               |Built-ins                                    |
|quit                          |       |       |                                                                                               |Built-ins                                    |
|range                         |       |X      |Looping over a range produces a classic for loop.                                              |Built-ins                                    |
|repr                          |       |       |                                                                                               |Built-ins                                    |
|reversed                      |       |       |                                                                                               |Built-ins                                    |
|round                         |       |       |                                                                                               |Built-ins                                    |
|set                           |       |       |                                                                                               |Built-ins                                    |
|setattr                       |       |       |                                                                                               |Built-ins                                    |
|slice                         |       |       |                                                                                               |Built-ins                                    |
|sorted                        |       |       |                                                                                               |Built-ins                                    |
|staticmethod                  |       |       |                                                                                               |Built-ins                                    |
|str                           |       |X      |Literal support exists. Function support untested.                                             |Built-ins                                    |
|sum                           |       |       |                                                                                               |Built-ins                                    |
|super                         |       |       |                                                                                               |Built-ins                                    |
|tuple                         |       |X      |Limited literal support. Function support untested.                                            |Built-ins                                    |
|type                          |       |       |                                                                                               |Built-ins                                    |
|vars                          |       |       |                                                                                               |Built-ins                                    |
|zip                           |       |       |                                                                                               |Built-ins                                    |
|Add                           |       |X      |Handles addition and integers. Strings untested.                                               |Operators                                    |
|Sub                           |X      |       |                                                                                               |Operators                                    |
|Mult                          |X      |       |                                                                                               |Operators                                    |
|MatMult                       |       |       |                                                                                               |Operators                                    |
|Div                           |X      |       |                                                                                               |Operators                                    |
|Mod                           |       |X      |Missing tests.                                                                                 |Operators                                    |
|Pow                           |X      |       |                                                                                               |Operators                                    |
|LShift                        |       |X      |Missing tests.                                                                                 |Operators                                    |
|RShift                        |       |X      |Missing tests.                                                                                 |Operators                                    |
|BitOr                         |       |X      |Missing tests.                                                                                 |Operators                                    |
|BitXor                        |       |X      |Missing tests.                                                                                 |Operators                                    |
|BitAnd                        |       |X      |Missing tests.                                                                                 |Operators                                    |
|FloorDiv                      |X      |       |                                                                                               |Operators                                    |
|Annotated                     |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Any                           |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Callable                      |       |       |                                                                                               |Typing - Super-special typing primitives     |
|ClassVar                      |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Concatenate                   |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Final                         |       |       |                                                                                               |Typing - Super-special typing primitives     |
|ForwardRef                    |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Generic                       |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Literal                       |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Optional                      |       |       |                                                                                               |Typing - Super-special typing primitives     |
|ParamSpec                     |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Protocol                      |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Tuple                         |       |X      |See "tuple"                                                                                    |Typing - Super-special typing primitives     |
|Type                          |       |       |                                                                                               |Typing - Super-special typing primitives     |
|TypeVar                       |       |       |                                                                                               |Typing - Super-special typing primitives     |
|Union                         |       |       |                                                                                               |Typing - Super-special typing primitives     |
|AbstractSet                   |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|ByteString                    |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Container                     |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|ContextManager                |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Hashable                      |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|ItemsView                     |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Iterable                      |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Iterator                      |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|KeysView                      |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Mapping                       |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|MappingView                   |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|MutableMapping                |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|MutableSequence               |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|MutableSet                    |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Sequence                      |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Sized                         |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|ValuesView                    |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Awaitable                     |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|AsyncIterator                 |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|AsyncIterable                 |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Coroutine                     |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Collection                    |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|AsyncGenerator                |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|AsyncContextManager           |       |       |                                                                                               |Typing - ABCs (from collections.abc).        |
|Reversible                    |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsAbs                   |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsBytes                 |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsComplex               |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsFloat                 |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsIndex                 |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsInt                   |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|SupportsRound                 |       |       |                                                                                               |Typing - Structural checks, a.k.a. protocols.|
|ChainMap                      |       |       |                                                                                               |Typing - Concrete collection types.          |
|Counter                       |       |       |                                                                                               |Typing - Concrete collection types.          |
|Deque                         |       |       |                                                                                               |Typing - Concrete collection types.          |
|Dict                          |       |       |                                                                                               |Typing - Concrete collection types.          |
|DefaultDict                   |       |       |                                                                                               |Typing - Concrete collection types.          |
|List                          |       |X      |See "list"                                                                                     |Typing - Concrete collection types.          |
|OrderedDict                   |       |       |                                                                                               |Typing - Concrete collection types.          |
|Set                           |       |       |                                                                                               |Typing - Concrete collection types.          |
|FrozenSet                     |       |       |                                                                                               |Typing - Concrete collection types.          |
|NamedTuple                    |       |       |Not really a type.                                                                             |Typing - Concrete collection types.          |
|TypedDict                     |       |       |Not really a type.                                                                             |Typing - Concrete collection types.          |
|Generator                     |       |       |                                                                                               |Typing - Concrete collection types.          |
|BinaryIO                      |       |       |                                                                                               |Typing - Other concrete types.               |
|IO                            |       |       |                                                                                               |Typing - Other concrete types.               |
|Match                         |       |       |                                                                                               |Typing - Other concrete types.               |
|Pattern                       |       |       |                                                                                               |Typing - Other concrete types.               |
|TextIO                        |       |       |                                                                                               |Typing - Other concrete types.               |
|AnyStr                        |       |       |                                                                                               |Typing - One-off things.                     |
|NewType                       |       |       |                                                                                               |Typing - One-off things.                     |
|NoReturn                      |       |       |                                                                                               |Typing - One-off things.                     |
|ParamSpecArgs                 |       |       |                                                                                               |Typing - One-off things.                     |
|ParamSpecKwargs               |       |       |                                                                                               |Typing - One-off things.                     |
|TypeAlias                     |       |       |                                                                                               |Typing - One-off things.                     |
|TypeGuard                     |       |       |                                                                                               |Typing - One-off things.                     |
|abc                           |       |       |                                                                                               |Standard Library Modules                     |
|aifc                          |       |       |                                                                                               |Standard Library Modules                     |
|antigravity                   |       |       |                                                                                               |Standard Library Modules                     |
|argparse                      |       |       |                                                                                               |Standard Library Modules                     |
|array                         |       |       |                                                                                               |Standard Library Modules                     |
|ast                           |       |       |Too meta?                                                                                      |Standard Library Modules                     |
|asynchat                      |       |       |                                                                                               |Standard Library Modules                     |
|asyncio                       |       |       |                                                                                               |Standard Library Modules                     |
|asyncore                      |       |       |                                                                                               |Standard Library Modules                     |
|atexit                        |       |       |                                                                                               |Standard Library Modules                     |
|audioop                       |       |       |                                                                                               |Standard Library Modules                     |
|backend_interagg              |       |       |                                                                                               |Standard Library Modules                     |
|base64                        |       |       |                                                                                               |Standard Library Modules                     |
|bdb                           |       |       |                                                                                               |Standard Library Modules                     |
|binascii                      |       |       |                                                                                               |Standard Library Modules                     |
|binhex                        |       |       |                                                                                               |Standard Library Modules                     |
|bisect                        |       |       |                                                                                               |Standard Library Modules                     |
|builtins                      |       |       |                                                                                               |Standard Library Modules                     |
|bz2                           |       |       |                                                                                               |Standard Library Modules                     |
|cProfile                      |       |       |                                                                                               |Standard Library Modules                     |
|calendar                      |       |       |                                                                                               |Standard Library Modules                     |
|certifi                       |       |       |                                                                                               |Standard Library Modules                     |
|cgi                           |       |       |                                                                                               |Standard Library Modules                     |
|cgitb                         |       |       |                                                                                               |Standard Library Modules                     |
|chardet                       |       |       |                                                                                               |Standard Library Modules                     |
|chunk                         |       |       |                                                                                               |Standard Library Modules                     |
|cmath                         |       |       |                                                                                               |Standard Library Modules                     |
|cmd                           |       |       |                                                                                               |Standard Library Modules                     |
|code                          |       |       |                                                                                               |Standard Library Modules                     |
|codecs                        |       |       |                                                                                               |Standard Library Modules                     |
|codeop                        |       |       |                                                                                               |Standard Library Modules                     |
|collections                   |       |       |                                                                                               |Standard Library Modules                     |
|colorsys                      |       |       |                                                                                               |Standard Library Modules                     |
|compileall                    |       |       |                                                                                               |Standard Library Modules                     |
|concurrent                    |       |       |                                                                                               |Standard Library Modules                     |
|configparser                  |       |       |                                                                                               |Standard Library Modules                     |
|contextlib                    |       |       |                                                                                               |Standard Library Modules                     |
|contextvars                   |       |       |                                                                                               |Standard Library Modules                     |
|copy                          |       |       |                                                                                               |Standard Library Modules                     |
|copyreg                       |       |       |                                                                                               |Standard Library Modules                     |
|crypt                         |       |       |                                                                                               |Standard Library Modules                     |
|csv                           |       |       |                                                                                               |Standard Library Modules                     |
|ctypes                        |       |       |                                                                                               |Standard Library Modules                     |
|curses                        |       |       |                                                                                               |Standard Library Modules                     |
|dataclasses                   |       |       |                                                                                               |Standard Library Modules                     |
|datalore                      |       |       |                                                                                               |Standard Library Modules                     |
|datetime                      |       |       |                                                                                               |Standard Library Modules                     |
|dbm                           |       |       |                                                                                               |Standard Library Modules                     |
|decimal                       |       |       |                                                                                               |Standard Library Modules                     |
|difflib                       |       |       |                                                                                               |Standard Library Modules                     |
|dis                           |       |       |                                                                                               |Standard Library Modules                     |
|distutils                     |       |       |                                                                                               |Standard Library Modules                     |
|doctest                       |       |       |                                                                                               |Standard Library Modules                     |
|email                         |       |       |                                                                                               |Standard Library Modules                     |
|encodings                     |       |       |                                                                                               |Standard Library Modules                     |
|ensurepip                     |       |       |                                                                                               |Standard Library Modules                     |
|enum                          |       |       |                                                                                               |Standard Library Modules                     |
|errno                         |       |       |                                                                                               |Standard Library Modules                     |
|faulthandler                  |       |       |                                                                                               |Standard Library Modules                     |
|filecmp                       |       |       |                                                                                               |Standard Library Modules                     |
|fileinput                     |       |       |                                                                                               |Standard Library Modules                     |
|fnmatch                       |       |       |                                                                                               |Standard Library Modules                     |
|fractions                     |       |       |                                                                                               |Standard Library Modules                     |
|ftplib                        |       |       |                                                                                               |Standard Library Modules                     |
|functools                     |       |       |                                                                                               |Standard Library Modules                     |
|gc                            |       |       |                                                                                               |Standard Library Modules                     |
|genericpath                   |       |       |                                                                                               |Standard Library Modules                     |
|getopt                        |       |       |                                                                                               |Standard Library Modules                     |
|getpass                       |       |       |                                                                                               |Standard Library Modules                     |
|gettext                       |       |       |                                                                                               |Standard Library Modules                     |
|glob                          |       |       |                                                                                               |Standard Library Modules                     |
|graphlib                      |       |       |                                                                                               |Standard Library Modules                     |
|gzip                          |       |       |                                                                                               |Standard Library Modules                     |
|hashlib                       |       |       |                                                                                               |Standard Library Modules                     |
|heapq                         |       |       |                                                                                               |Standard Library Modules                     |
|hmac                          |       |       |                                                                                               |Standard Library Modules                     |
|html                          |       |       |                                                                                               |Standard Library Modules                     |
|http                          |       |       |                                                                                               |Standard Library Modules                     |
|idlelib                       |       |       |                                                                                               |Standard Library Modules                     |
|idna                          |       |       |                                                                                               |Standard Library Modules                     |
|imaplib                       |       |       |                                                                                               |Standard Library Modules                     |
|imghdr                        |       |       |                                                                                               |Standard Library Modules                     |
|imp                           |       |       |                                                                                               |Standard Library Modules                     |
|importlib                     |       |       |                                                                                               |Standard Library Modules                     |
|inspect                       |       |       |                                                                                               |Standard Library Modules                     |
|interpreterInfo               |       |       |                                                                                               |Standard Library Modules                     |
|io                            |       |       |                                                                                               |Standard Library Modules                     |
|ipaddress                     |       |       |                                                                                               |Standard Library Modules                     |
|itertools                     |       |       |                                                                                               |Standard Library Modules                     |
|json                          |       |       |                                                                                               |Standard Library Modules                     |
|keyword                       |       |       |                                                                                               |Standard Library Modules                     |
|lib2to3                       |       |       |                                                                                               |Standard Library Modules                     |
|linecache                     |       |       |                                                                                               |Standard Library Modules                     |
|locale                        |       |       |                                                                                               |Standard Library Modules                     |
|logging                       |       |       |                                                                                               |Standard Library Modules                     |
|lzma                          |       |       |                                                                                               |Standard Library Modules                     |
|mailbox                       |       |       |                                                                                               |Standard Library Modules                     |
|mailcap                       |       |       |                                                                                               |Standard Library Modules                     |
|marshal                       |       |       |                                                                                               |Standard Library Modules                     |
|math                          |       |X      |Many functions supported. Must have math imported as math.                                     |Standard Library Modules                     |
|mimetypes                     |       |       |                                                                                               |Standard Library Modules                     |
|mmap                          |       |       |                                                                                               |Standard Library Modules                     |
|modulefinder                  |       |       |                                                                                               |Standard Library Modules                     |
|msilib                        |       |       |                                                                                               |Standard Library Modules                     |
|msvcrt                        |       |       |                                                                                               |Standard Library Modules                     |
|multiprocessing               |       |       |                                                                                               |Standard Library Modules                     |
|netrc                         |       |       |                                                                                               |Standard Library Modules                     |
|nntplib                       |       |       |                                                                                               |Standard Library Modules                     |
|nt                            |       |       |                                                                                               |Standard Library Modules                     |
|ntpath                        |       |       |                                                                                               |Standard Library Modules                     |
|nturl2path                    |       |       |                                                                                               |Standard Library Modules                     |
|numbers                       |       |       |                                                                                               |Standard Library Modules                     |
|opcode                        |       |       |                                                                                               |Standard Library Modules                     |
|operator                      |       |       |                                                                                               |Standard Library Modules                     |
|optparse                      |       |       |                                                                                               |Standard Library Modules                     |
|os                            |       |       |                                                                                               |Standard Library Modules                     |
|pathlib                       |       |       |                                                                                               |Standard Library Modules                     |
|pdb                           |       |       |                                                                                               |Standard Library Modules                     |
|pickle                        |       |       |                                                                                               |Standard Library Modules                     |
|pickletools                   |       |       |                                                                                               |Standard Library Modules                     |
|pip                           |       |       |                                                                                               |Standard Library Modules                     |
|pipes                         |       |       |                                                                                               |Standard Library Modules                     |
|pkg_resources                 |       |       |                                                                                               |Standard Library Modules                     |
|pkgutil                       |       |       |                                                                                               |Standard Library Modules                     |
|platform                      |       |       |                                                                                               |Standard Library Modules                     |
|plistlib                      |       |       |                                                                                               |Standard Library Modules                     |
|poplib                        |       |       |                                                                                               |Standard Library Modules                     |
|posixpath                     |       |       |                                                                                               |Standard Library Modules                     |
|pprint                        |       |       |                                                                                               |Standard Library Modules                     |
|profile                       |       |       |                                                                                               |Standard Library Modules                     |
|pstats                        |       |       |                                                                                               |Standard Library Modules                     |
|pty                           |       |       |                                                                                               |Standard Library Modules                     |
|py_compile                    |       |       |                                                                                               |Standard Library Modules                     |
|pyclbr                        |       |       |                                                                                               |Standard Library Modules                     |
|pycompletionserver            |       |       |                                                                                               |Standard Library Modules                     |
|pydev_app_engine_debug_startup|       |       |                                                                                               |Standard Library Modules                     |
|pydev_console                 |       |       |                                                                                               |Standard Library Modules                     |
|pydev_coverage                |       |       |                                                                                               |Standard Library Modules                     |
|pydev_ipython                 |       |       |                                                                                               |Standard Library Modules                     |
|pydev_pysrc                   |       |       |                                                                                               |Standard Library Modules                     |
|pydev_test_pydevd_reload      |       |       |                                                                                               |Standard Library Modules                     |
|pydev_tests                   |       |       |                                                                                               |Standard Library Modules                     |
|pydev_tests_mainloop          |       |       |                                                                                               |Standard Library Modules                     |
|pydev_tests_python            |       |       |                                                                                               |Standard Library Modules                     |
|pydevconsole                  |       |       |                                                                                               |Standard Library Modules                     |
|pydevd                        |       |       |                                                                                               |Standard Library Modules                     |
|pydevd_concurrency_analyser   |       |       |                                                                                               |Standard Library Modules                     |
|pydevd_file_utils             |       |       |                                                                                               |Standard Library Modules                     |
|pydevd_plugins                |       |       |                                                                                               |Standard Library Modules                     |
|pydevd_pycharm                |       |       |                                                                                               |Standard Library Modules                     |
|pydevd_tracing                |       |       |                                                                                               |Standard Library Modules                     |
|pydoc                         |       |       |                                                                                               |Standard Library Modules                     |
|pydoc_data                    |       |       |                                                                                               |Standard Library Modules                     |
|pyexpat                       |       |       |                                                                                               |Standard Library Modules                     |
|pythagoras                    |       |       |                                                                                               |Standard Library Modules                     |
|queue                         |       |       |                                                                                               |Standard Library Modules                     |
|quopri                        |       |       |                                                                                               |Standard Library Modules                     |
|random                        |       |       |                                                                                               |Standard Library Modules                     |
|re                            |       |       |                                                                                               |Standard Library Modules                     |
|reprlib                       |       |       |                                                                                               |Standard Library Modules                     |
|requests                      |       |       |                                                                                               |Standard Library Modules                     |
|rlcompleter                   |       |       |                                                                                               |Standard Library Modules                     |
|runfiles                      |       |       |                                                                                               |Standard Library Modules                     |
|runpy                         |       |       |                                                                                               |Standard Library Modules                     |
|sched                         |       |       |                                                                                               |Standard Library Modules                     |
|secrets                       |       |       |                                                                                               |Standard Library Modules                     |
|select                        |       |       |                                                                                               |Standard Library Modules                     |
|selectors                     |       |       |                                                                                               |Standard Library Modules                     |
|setup                         |       |       |                                                                                               |Standard Library Modules                     |
|setup_cython                  |       |       |                                                                                               |Standard Library Modules                     |
|setuptools                    |       |       |                                                                                               |Standard Library Modules                     |
|shelve                        |       |       |                                                                                               |Standard Library Modules                     |
|shlex                         |       |       |                                                                                               |Standard Library Modules                     |
|shutil                        |       |       |                                                                                               |Standard Library Modules                     |
|signal                        |       |       |                                                                                               |Standard Library Modules                     |
|site                          |       |       |                                                                                               |Standard Library Modules                     |
|sitecustomize                 |       |       |                                                                                               |Standard Library Modules                     |
|smtpd                         |       |       |                                                                                               |Standard Library Modules                     |
|smtplib                       |       |       |                                                                                               |Standard Library Modules                     |
|sndhdr                        |       |       |                                                                                               |Standard Library Modules                     |
|socket                        |       |       |                                                                                               |Standard Library Modules                     |
|socketserver                  |       |       |                                                                                               |Standard Library Modules                     |
|sqlite3                       |       |       |                                                                                               |Standard Library Modules                     |
|sre_compile                   |       |       |                                                                                               |Standard Library Modules                     |
|sre_constants                 |       |       |                                                                                               |Standard Library Modules                     |
|sre_parse                     |       |       |                                                                                               |Standard Library Modules                     |
|ssl                           |       |       |                                                                                               |Standard Library Modules                     |
|stat                          |       |       |                                                                                               |Standard Library Modules                     |
|statistics                    |       |       |                                                                                               |Standard Library Modules                     |
|string                        |       |       |                                                                                               |Standard Library Modules                     |
|stringprep                    |       |       |                                                                                               |Standard Library Modules                     |
|struct                        |       |       |                                                                                               |Standard Library Modules                     |
|subprocess                    |       |       |                                                                                               |Standard Library Modules                     |
|sunau                         |       |       |                                                                                               |Standard Library Modules                     |
|symtable                      |       |       |                                                                                               |Standard Library Modules                     |
|sys                           |       |       |                                                                                               |Standard Library Modules                     |
|sysconfig                     |       |       |                                                                                               |Standard Library Modules                     |
|tabnanny                      |       |       |                                                                                               |Standard Library Modules                     |
|tarfile                       |       |       |                                                                                               |Standard Library Modules                     |
|telnetlib                     |       |       |                                                                                               |Standard Library Modules                     |
|tempfile                      |       |       |                                                                                               |Standard Library Modules                     |
|test                          |       |       |                                                                                               |Standard Library Modules                     |
|textwrap                      |       |       |                                                                                               |Standard Library Modules                     |
|this                          |       |       |                                                                                               |Standard Library Modules                     |
|threading                     |       |       |                                                                                               |Standard Library Modules                     |
|time                          |       |       |                                                                                               |Standard Library Modules                     |
|timeit                        |       |       |                                                                                               |Standard Library Modules                     |
|tkinter                       |       |       |                                                                                               |Standard Library Modules                     |
|token                         |       |       |                                                                                               |Standard Library Modules                     |
|tokenize                      |       |       |                                                                                               |Standard Library Modules                     |
|trace                         |       |       |                                                                                               |Standard Library Modules                     |
|traceback                     |       |       |                                                                                               |Standard Library Modules                     |
|tracemalloc                   |       |       |                                                                                               |Standard Library Modules                     |
|tty                           |       |       |                                                                                               |Standard Library Modules                     |
|turtle                        |       |       |                                                                                               |Standard Library Modules                     |
|turtledemo                    |       |       |                                                                                               |Standard Library Modules                     |
|types                         |       |       |                                                                                               |Standard Library Modules                     |
|typing                        |       |       |                                                                                               |Standard Library Modules                     |
|unicodedata                   |       |       |                                                                                               |Standard Library Modules                     |
|unittest                      |       |       |                                                                                               |Standard Library Modules                     |
|urllib                        |       |       |                                                                                               |Standard Library Modules                     |
|urllib3                       |       |       |                                                                                               |Standard Library Modules                     |
|uu                            |       |       |                                                                                               |Standard Library Modules                     |
|uuid                          |       |       |                                                                                               |Standard Library Modules                     |
|venv                          |       |       |                                                                                               |Standard Library Modules                     |
|warnings                      |       |       |                                                                                               |Standard Library Modules                     |
|wave                          |       |       |                                                                                               |Standard Library Modules                     |
|weakref                       |       |       |                                                                                               |Standard Library Modules                     |
|webbrowser                    |       |       |                                                                                               |Standard Library Modules                     |
|winreg                        |       |       |                                                                                               |Standard Library Modules                     |
|winsound                      |       |       |                                                                                               |Standard Library Modules                     |
|wsgiref                       |       |       |                                                                                               |Standard Library Modules                     |
|xdrlib                        |       |       |                                                                                               |Standard Library Modules                     |
|xml                           |       |       |                                                                                               |Standard Library Modules                     |
|xmlrpc                        |       |       |                                                                                               |Standard Library Modules                     |
|xxsubtype                     |       |       |                                                                                               |Standard Library Modules                     |
|zipapp                        |       |       |                                                                                               |Standard Library Modules                     |
|zipfile                       |       |       |                                                                                               |Standard Library Modules                     |
|zipimport                     |       |       |                                                                                               |Standard Library Modules                     |
|zlib                          |       |       |                                                                                               |Standard Library Modules                     |
|zoneinfo                      |       |       |                                                                                               |Standard Library Modules                     |
|requests                      |       |X      |Experimental support for a simple "get" request                                                |Third Party                                  |

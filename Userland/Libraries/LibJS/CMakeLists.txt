set(SOURCES
    AST.cpp
    Bytecode/ASTCodegen.cpp
    Bytecode/BasicBlock.cpp
    Bytecode/Generator.cpp
    Bytecode/Instruction.cpp
    Bytecode/Interpreter.cpp
    Bytecode/Op.cpp
    Bytecode/Pass/DumpCFG.cpp
    Bytecode/Pass/GenerateCFG.cpp
    Bytecode/Pass/MergeBlocks.cpp
    Bytecode/Pass/PlaceBlocks.cpp
    Bytecode/Pass/UnifySameBlocks.cpp
    Bytecode/StringTable.cpp
    Console.cpp
    Heap/BlockAllocator.cpp
    Heap/CellAllocator.cpp
    Heap/Handle.cpp
    Heap/Heap.cpp
    Heap/HeapBlock.cpp
    Interpreter.cpp
    Lexer.cpp
    MarkupGenerator.cpp
    Parser.cpp
    Runtime/AbstractOperations.cpp
    Runtime/AggregateError.cpp
    Runtime/AggregateErrorConstructor.cpp
    Runtime/AggregateErrorPrototype.cpp
    Runtime/ArgumentsObject.cpp
    Runtime/Array.cpp
    Runtime/ArrayBuffer.cpp
    Runtime/ArrayBufferConstructor.cpp
    Runtime/ArrayBufferPrototype.cpp
    Runtime/ArrayConstructor.cpp
    Runtime/ArrayIterator.cpp
    Runtime/ArrayIteratorPrototype.cpp
    Runtime/ArrayPrototype.cpp
    Runtime/AtomicsObject.cpp
    Runtime/BigInt.cpp
    Runtime/BigIntConstructor.cpp
    Runtime/BigIntObject.cpp
    Runtime/BigIntPrototype.cpp
    Runtime/BooleanConstructor.cpp
    Runtime/BooleanObject.cpp
    Runtime/BooleanPrototype.cpp
    Runtime/BoundFunction.cpp
    Runtime/ConsoleObject.cpp
    Runtime/DataView.cpp
    Runtime/DataViewConstructor.cpp
    Runtime/DataViewPrototype.cpp
    Runtime/Date.cpp
    Runtime/DateConstructor.cpp
    Runtime/DatePrototype.cpp
    Runtime/DeclarativeEnvironment.cpp
    Runtime/Environment.cpp
    Runtime/Error.cpp
    Runtime/ErrorConstructor.cpp
    Runtime/ErrorPrototype.cpp
    Runtime/ErrorTypes.cpp
    Runtime/Exception.cpp
    Runtime/FinalizationRegistry.cpp
    Runtime/FinalizationRegistryConstructor.cpp
    Runtime/FinalizationRegistryPrototype.cpp
    Runtime/FunctionConstructor.cpp
    Runtime/FunctionEnvironment.cpp
    Runtime/FunctionObject.cpp
    Runtime/FunctionPrototype.cpp
    Runtime/GeneratorFunctionConstructor.cpp
    Runtime/GeneratorFunctionPrototype.cpp
    Runtime/GeneratorObject.cpp
    Runtime/GeneratorObjectPrototype.cpp
    Runtime/GlobalEnvironment.cpp
    Runtime/GlobalObject.cpp
    Runtime/IndexedProperties.cpp
    Runtime/Intl/Intl.cpp
    Runtime/IteratorOperations.cpp
    Runtime/IteratorPrototype.cpp
    Runtime/JSONObject.cpp
    Runtime/Map.cpp
    Runtime/MapConstructor.cpp
    Runtime/MapIterator.cpp
    Runtime/MapIteratorPrototype.cpp
    Runtime/MapPrototype.cpp
    Runtime/MarkedValueList.cpp
    Runtime/MathObject.cpp
    Runtime/NativeFunction.cpp
    Runtime/NumberConstructor.cpp
    Runtime/NumberObject.cpp
    Runtime/NumberPrototype.cpp
    Runtime/Object.cpp
    Runtime/ObjectConstructor.cpp
    Runtime/ObjectEnvironment.cpp
    Runtime/ObjectPrototype.cpp
    Runtime/OrdinaryFunctionObject.cpp
    Runtime/PrimitiveString.cpp
    Runtime/Promise.cpp
    Runtime/PromiseConstructor.cpp
    Runtime/PromiseJobs.cpp
    Runtime/PromisePrototype.cpp
    Runtime/PromiseReaction.cpp
    Runtime/PromiseResolvingFunction.cpp
    Runtime/PropertyDescriptor.cpp
    Runtime/ProxyConstructor.cpp
    Runtime/ProxyObject.cpp
    Runtime/Reference.cpp
    Runtime/ReflectObject.cpp
    Runtime/RegExpConstructor.cpp
    Runtime/RegExpObject.cpp
    Runtime/RegExpPrototype.cpp
    Runtime/RegExpStringIterator.cpp
    Runtime/RegExpStringIteratorPrototype.cpp
    Runtime/Set.cpp
    Runtime/SetConstructor.cpp
    Runtime/SetIterator.cpp
    Runtime/SetIteratorPrototype.cpp
    Runtime/SetPrototype.cpp
    Runtime/Shape.cpp
    Runtime/StringConstructor.cpp
    Runtime/StringIterator.cpp
    Runtime/StringIteratorPrototype.cpp
    Runtime/StringObject.cpp
    Runtime/StringPrototype.cpp
    Runtime/Symbol.cpp
    Runtime/SymbolConstructor.cpp
    Runtime/SymbolObject.cpp
    Runtime/SymbolPrototype.cpp
    Runtime/Temporal/AbstractOperations.cpp
    Runtime/Temporal/Calendar.cpp
    Runtime/Temporal/CalendarConstructor.cpp
    Runtime/Temporal/CalendarPrototype.cpp
    Runtime/Temporal/Duration.cpp
    Runtime/Temporal/DurationConstructor.cpp
    Runtime/Temporal/DurationPrototype.cpp
    Runtime/Temporal/Instant.cpp
    Runtime/Temporal/InstantConstructor.cpp
    Runtime/Temporal/InstantPrototype.cpp
    Runtime/Temporal/Now.cpp
    Runtime/Temporal/PlainDate.cpp
    Runtime/Temporal/PlainDateConstructor.cpp
    Runtime/Temporal/PlainDatePrototype.cpp
    Runtime/Temporal/PlainDateTime.cpp
    Runtime/Temporal/PlainDateTimeConstructor.cpp
    Runtime/Temporal/PlainDateTimePrototype.cpp
    Runtime/Temporal/PlainMonthDay.cpp
    Runtime/Temporal/PlainMonthDayConstructor.cpp
    Runtime/Temporal/PlainMonthDayPrototype.cpp
    Runtime/Temporal/PlainTime.cpp
    Runtime/Temporal/PlainTimeConstructor.cpp
    Runtime/Temporal/PlainTimePrototype.cpp
    Runtime/Temporal/PlainYearMonth.cpp
    Runtime/Temporal/PlainYearMonthConstructor.cpp
    Runtime/Temporal/PlainYearMonthPrototype.cpp
    Runtime/Temporal/Temporal.cpp
    Runtime/Temporal/TimeZone.cpp
    Runtime/Temporal/TimeZoneConstructor.cpp
    Runtime/Temporal/TimeZonePrototype.cpp
    Runtime/Temporal/ZonedDateTime.cpp
    Runtime/Temporal/ZonedDateTimeConstructor.cpp
    Runtime/Temporal/ZonedDateTimePrototype.cpp
    Runtime/TypedArray.cpp
    Runtime/TypedArrayConstructor.cpp
    Runtime/TypedArrayPrototype.cpp
    Runtime/Utf16String.cpp
    Runtime/Value.cpp
    Runtime/VM.cpp
    Runtime/WeakContainer.cpp
    Runtime/WeakMap.cpp
    Runtime/WeakMapConstructor.cpp
    Runtime/WeakMapPrototype.cpp
    Runtime/WeakRef.cpp
    Runtime/WeakRefConstructor.cpp
    Runtime/WeakRefPrototype.cpp
    Runtime/WeakSet.cpp
    Runtime/WeakSetConstructor.cpp
    Runtime/WeakSetPrototype.cpp
    SyntaxHighlighter.cpp
    Token.cpp
)

serenity_lib(LibJS js)
target_link_libraries(LibJS LibM LibCore LibCrypto LibRegex LibSyntax LibUnicode)

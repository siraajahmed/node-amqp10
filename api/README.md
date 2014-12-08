#Index

**Classes**

* [class: NodeSbusEventHubAdapter](#NodeSbusEventHubAdapter)
  * [new NodeSbusEventHubAdapter()](#new_NodeSbusEventHubAdapter)
* [class: Codec](#Codec)
  * [new Codec()](#new_Codec)
  * [codec._readFullValue(buf, [offset], [doNotConsume], [forcedCode])](#Codec#_readFullValue)
  * [codec.decode(buf, [offset], [forcedCode])](#Codec#decode)
  * [codec.encode(val, buf, [forceType])](#Codec#encode)
* [class: Connection](#Connection)
  * [new Connection(connectPolicy)](#new_Connection)
  * [connection.open(address, sasl)](#Connection#open)
* [class: MalformedHeaderError](#MalformedHeaderError)
  * [new MalformedHeaderError(msg)](#new_MalformedHeaderError)
* [class: NotImplementedError](#NotImplementedError)
  * [new NotImplementedError(msg)](#new_NotImplementedError)
* [class: MalformedPayloadError](#MalformedPayloadError)
  * [new MalformedPayloadError(msg)](#new_MalformedPayloadError)
* [class: EncodingError](#EncodingError)
  * [new EncodingError(msg)](#new_EncodingError)
* [class: OverCapacityError](#OverCapacityError)
  * [new OverCapacityError(msg)](#new_OverCapacityError)
* [class: AuthenticationError](#AuthenticationError)
  * [new AuthenticationError(msg)](#new_AuthenticationError)
* [class: ArgumentError](#ArgumentError)
  * [new ArgumentError(arg)](#new_ArgumentError)
* [class: InvalidStateError](#InvalidStateError)
  * [new InvalidStateError(msg)](#new_InvalidStateError)
* [class: AttachFrame](#AttachFrame)
  * [new AttachFrame()](#new_AttachFrame)
* [class: BeginFrame](#BeginFrame)
  * [new BeginFrame()](#new_BeginFrame)
* [class: CloseFrame](#CloseFrame)
  * [new CloseFrame()](#new_CloseFrame)
* [class: DetachFrame](#DetachFrame)
  * [new DetachFrame()](#new_DetachFrame)
* [class: DispositionFrame](#DispositionFrame)
  * [new DispositionFrame()](#new_DispositionFrame)
* [class: EndFrame](#EndFrame)
  * [new EndFrame()](#new_EndFrame)
* [class: FlowFrame](#FlowFrame)
  * [new FlowFrame()](#new_FlowFrame)
* [class: Frame](#Frame)
  * [new Frame()](#new_Frame)
  * [frame.outgoing()](#Frame#outgoing)
  * [frame.readPerformative(describedType)](#Frame#readPerformative)
* [class: AMQPFrame](#AMQPFrame)
  * [new AMQPFrame()](#new_AMQPFrame)
  * [aMQPFrame._getPerformative()](#AMQPFrame#_getPerformative)
  * [aMQPFrame._getAdditionalPayload()](#AMQPFrame#_getAdditionalPayload)
* [class: FrameReader](#FrameReader)
  * [frameReader.read(cbuf)](#FrameReader#read)
  * [frameReader._readMessage(messageBuf)](#FrameReader#_readMessage)
* [class: OpenFrame](#OpenFrame)
  * [new OpenFrame()](#new_OpenFrame)
* [class: SaslFrame](#SaslFrame)
  * [new SaslFrame()](#new_SaslFrame)
* [class: SaslMechanisms](#SaslMechanisms)
  * [new SaslMechanisms(options)](#new_SaslMechanisms)
* [class: SaslInit](#SaslInit)
  * [new SaslInit(options)](#new_SaslInit)
* [class: SaslChallenge](#SaslChallenge)
  * [new SaslChallenge(options)](#new_SaslChallenge)
* [class: SaslResponse](#SaslResponse)
  * [new SaslResponse(options)](#new_SaslResponse)
* [class: SaslOutcome](#SaslOutcome)
  * [new SaslOutcome(options)](#new_SaslOutcome)
* [class: TransferFrame](#TransferFrame)
  * [new TransferFrame()](#new_TransferFrame)
* [class: PolicyBase](#PolicyBase)
  * [new PolicyBase()](#new_PolicyBase)
* [class: Sasl](#Sasl)
  * [new Sasl()](#new_Sasl)
* [class: Session](#Session)
  * [new Session(conn)](#new_Session)
  * [session.sendMessage(link, message, options)](#Session#sendMessage)
* [class: Types](#Types)
  * [new Types()](#new_Types)
  * [types._listBuilder(val, bufb, codec, [width])](#Types#_listBuilder)
  * [types._arrayBuilder(val, bufb, codec, [width])](#Types#_arrayBuilder)
  * [types._mapBuilder(val, bufb, codec, [width])](#Types#_mapBuilder)
  * [types._initTypesArray()](#Types#_initTypesArray)
  * [types._initEncodersDecoders()](#Types#_initEncodersDecoders)
* [class: AMQPArray](#AMQPArray)
  * [new AMQPArray(arr, elementType)](#new_AMQPArray)
* [class: DescribedType](#DescribedType)
  * [new DescribedType(descriptor, value)](#new_DescribedType)
* [class: ForcedType](#ForcedType)
  * [new ForcedType(typeName, value)](#new_ForcedType)
* [class: Header](#Header)
  * [new Header(options)](#new_Header)
* [class: DeliveryAnnotations](#DeliveryAnnotations)
  * [new DeliveryAnnotations(annotations)](#new_DeliveryAnnotations)
* [class: Annotations](#Annotations)
  * [new Annotations(annotations)](#new_Annotations)
* [class: Properties](#Properties)
  * [new Properties(options)](#new_Properties)
* [class: ApplicationProperties](#ApplicationProperties)
  * [new ApplicationProperties(properties)](#new_ApplicationProperties)
* [class: Footer](#Footer)
  * [new Footer(map)](#new_Footer)
* [class: Data](#Data)
  * [new Data(data)](#new_Data)
* [class: AMQPSequence](#AMQPSequence)
  * [new AMQPSequence(values)](#new_AMQPSequence)
* [class: AMQPValue](#AMQPValue)
  * [new AMQPValue(value)](#new_AMQPValue)
* [class: Message](#Message)
  * [new Message(contents, body)](#new_Message)
* [class: Symbol](#Symbol)
  * [new Symbol(str)](#new_Symbol)

**Functions**

* [assertArguments(options, argnames)](#assertArguments)
* [encoder(val, buf, [codec])](#encoder)
* [decoder(buf, [codec])](#decoder)
* [onUndef(arg1, arg2)](#onUndef)
* [orDefaults(map, defaultMap)](#orDefaults)

**Members**

* [payload](#payload)
 
<a name="NodeSbusEventHubAdapter"></a>
#class: NodeSbusEventHubAdapter
**Members**

* [class: NodeSbusEventHubAdapter](#NodeSbusEventHubAdapter)
  * [new NodeSbusEventHubAdapter()](#new_NodeSbusEventHubAdapter)

<a name="new_NodeSbusEventHubAdapter"></a>
##new NodeSbusEventHubAdapter()
Adapts node-amqp-1-0 to adhere to the interface defined by the node-sbus adapter,
for EventHub support.  Defines "subscribe" and "message" events, and builds
a messenger.

<a name="Codec"></a>
#class: Codec
**Members**

* [class: Codec](#Codec)
  * [new Codec()](#new_Codec)
  * [codec._readFullValue(buf, [offset], [doNotConsume], [forcedCode])](#Codec#_readFullValue)
  * [codec.decode(buf, [offset], [forcedCode])](#Codec#decode)
  * [codec.encode(val, buf, [forceType])](#Codec#encode)

<a name="new_Codec"></a>
##new Codec()
Build a codec.

<a name="Codec#_readFullValue"></a>
##codec._readFullValue(buf, [offset], [doNotConsume], [forcedCode])
Reads a full value's worth of bytes from a circular or regular buffer, or returns undefined if not enough bytes are there.

**Params**

- buf `Buffer` | `CBuffer` - Buffer or circular buffer to read from.  If a Buffer is given, it is assumed to be full.  
- \[offset=0\] `integer` - Offset - only valid for Buffer, not CBuffer.  
- \[doNotConsume=false\] `boolean` - If set to true, will peek bytes instead of reading them - useful for leaving
- \[forcedCode\] `Number` - If given, first byte is not assumed to be code and given code will be used - useful for arrays.  

**Returns**: `Array` - Buffer of full value + number of bytes read.
**Access**: private  
<a name="Codec#decode"></a>
##codec.decode(buf, [offset], [forcedCode])
Decode a single entity from a buffer (starting at offset 0).  Only simple values currently supported.

**Params**

- buf `Buffer` | `CBuffer` - The buffer/circular buffer to decode.  Will decode a single value per call.  
- \[offset=0\] `Number` - The offset to read from (only used for Buffers).  
- \[forcedCode\] `Number` - If given, will not consume first byte for code and will instead use this as the code. Useful for arrays.  

**Returns**: `Array` - Single decoded value + number of bytes consumed.  
<a name="Codec#encode"></a>
##codec.encode(val, buf, [forceType])
Encode the given value as an AMQP 1.0 bitstring.
 They are DescribedTypes, in which case they will be encoded as such.
 They contain an encodeOrdering array, in which case they will be encoded as a <code>list</code> of their values
 They are Int64s, in which case they will be encoded as <code>longs</code>.

**Params**

- val  - Value to encode.  
- buf `builder` - buffer-builder to write into.  
- \[forceType\] `string` - If set, forces the encoder for the given type.  

<a name="Connection"></a>
#class: Connection
**Members**

* [class: Connection](#Connection)
  * [new Connection(connectPolicy)](#new_Connection)
  * [connection.open(address, sasl)](#Connection#open)

<a name="new_Connection"></a>
##new Connection(connectPolicy)
Connection states, from AMQP 1.0 spec:

 <dl>
 <dt>START</dt>
 <dd><p>In this state a Connection exists, but nothing has been sent or received. This is the
 state an implementation would be in immediately after performing a socket connect or
 socket accept.</p></dd>

 <dt>HDR-RCVD</dt>
 <dd><p>In this state the Connection header has been received from our peer, but we have not
 yet sent anything.</p></dd>

 <dt>HDR-SENT</dt>
 <dd><p>In this state the Connection header has been sent to our peer, but we have not yet
 received anything.</p></dd>

 <dt>OPEN-PIPE</dt>
 <dd><p>In this state we have sent both the Connection header and the open frame, but we have not yet received anything.
 </p></dd>

 <dt>OC-PIPE</dt>
 <dd><p>In this state we have sent the Connection header, the open
 frame, any pipelined Connection traffic, and the close frame,
 but we have not yet received anything.</p></dd>

 <dt>OPEN-RCVD</dt>
 <dd><p>In this state we have sent and received the Connection header, and received an
 open frame from our peer, but have not yet sent an
 open frame.</p></dd>

 <dt>OPEN-SENT</dt>
 <dd><p>In this state we have sent and received the Connection header, and sent an
 open frame to our peer, but have not yet received an
 open frame.</p></dd>

 <dt>CLOSE-PIPE</dt>
 <dd><p>In this state we have send and received the Connection header, sent an
 open frame, any pipelined Connection traffic, and the
 close frame, but we have not yet received an
 open frame.</p></dd>

 <dt>OPENED</dt>
 <dd><p>In this state the Connection header and the open frame
 have both been sent and received.</p></dd>

 <dt>CLOSE-RCVD</dt>
 <dd><p>In this state we have received a close frame indicating
 that our partner has initiated a close. This means we will never have to read anything
 more from this Connection, however we can continue to write frames onto the Connection.
 If desired, an implementation could do a TCP half-close at this point to shutdown the
 read side of the Connection.</p></dd>

 <dt>CLOSE-SENT</dt>
 <dd><p>In this state we have sent a close frame to our partner.
 It is illegal to write anything more onto the Connection, however there may still be
 incoming frames. If desired, an implementation could do a TCP half-close at this point
 to shutdown the write side of the Connection.</p></dd>

 <dt>DISCARDING</dt>
 <dd><p>The DISCARDING state is a variant of the CLOSE_SENT state where the
 close is triggered by an error. In this case any incoming frames on
 the connection MUST be silently discarded until the peer's close frame
 is received.</p></dd>

 <dt>END</dt>
 <dd><p>In this state it is illegal for either endpoint to write anything more onto the
 Connection. The Connection may be safely closed and discarded.</p></dd>
 </dl>

Connection negotiation state diagram from AMQP 1.0 spec:

 <pre>
              R:HDR +=======+ S:HDR             R:HDR[!=S:HDR]
           +--------| START |-----+    +--------------------------------+
           |        +=======+     |    |                                |
          \\|/                    \\|/   |                                |
      +==========+             +==========+ S:OPEN                      |
 +----| HDR-RCVD |             | HDR-SENT |------+                      |
 |    +==========+             +==========+      |      R:HDR[!=S:HDR]  |
 |   S:HDR |                      | R:HDR        |    +-----------------+
 |         +--------+      +------+              |    |                 |
 |                 \\|/    \\|/                   \\|/   |                 |
 |                +==========+               +-----------+ S:CLOSE      |
 |                | HDR-EXCH |               | OPEN-PIPE |----+         |
 |                +==========+               +-----------+    |         |
 |           R:OPEN |      | S:OPEN              | R:HDR      |         |
 |         +--------+      +------+      +-------+            |         |
 |        \\|/                    \\|/    \\|/                  \\|/        |
 |   +===========+             +===========+ S:CLOSE       +---------+  |
 |   | OPEN-RCVD |             | OPEN-SENT |-----+         | OC-PIPE |--+
 |   +===========+             +===========+     |         +---------+  |
 |  S:OPEN |                      | R:OPEN      \\|/           | R:HDR   |
 |         |       +========+     |          +------------+   |         |
 |         +----- >| OPENED |< ---+          | CLOSE-PIPE |< -+         |
 |                 +========+                +------------+             |
 |           R:CLOSE |    | S:CLOSE              | R:OPEN               |
 |         +---------+    +-------+              |                      |
 |        \\|/                    \\|/             |                      |
 |   +============+          +=============+     |                      |
 |   | CLOSE-RCVD |          | CLOSE-SENT* |< ---+                      |
 |   +============+          +=============+                            |
 | S:CLOSE |                      | R:CLOSE                             |
 |         |         +=====+      |                                     |
 |         +------- >| END |< ----+                                     |
 |                   +=====+                                            |
 |                     /|\                                              |
 |    S:HDR[!=R:HDR]    |                R:HDR[!=S:HDR]                 |
 +----------------------+-----------------------------------------------+

 </pre>

R:<b>CTRL</b> = Received <b>CTRL</b>

S:<b>CTRL</b> = Sent <b>CTRL</b>

Also could be DISCARDING if an error condition triggered the CLOSE

**Params**

- connectPolicy  - ConnectPolicy from a PolicyBase implementation  

<a name="Connection#open"></a>
##connection.open(address, sasl)
Open a connection to the given (parsed) address (@see `AMQPClient`).

**Params**

- address  - Contains at least protocol, host and port, may contain user/pass, path.  
- sasl  - If given, contains a "negotiate" method that, given address and a callback, will run through SASL negotiations.  

<a name="MalformedHeaderError"></a>
#class: MalformedHeaderError
**Members**

* [class: MalformedHeaderError](#MalformedHeaderError)
  * [new MalformedHeaderError(msg)](#new_MalformedHeaderError)

<a name="new_MalformedHeaderError"></a>
##new MalformedHeaderError(msg)
AMQP Header is malformed.

**Params**

- msg   

<a name="NotImplementedError"></a>
#class: NotImplementedError
**Members**

* [class: NotImplementedError](#NotImplementedError)
  * [new NotImplementedError(msg)](#new_NotImplementedError)

<a name="new_NotImplementedError"></a>
##new NotImplementedError(msg)
Method or feature is not yet implemented.

**Params**

- msg   

<a name="MalformedPayloadError"></a>
#class: MalformedPayloadError
**Members**

* [class: MalformedPayloadError](#MalformedPayloadError)
  * [new MalformedPayloadError(msg)](#new_MalformedPayloadError)

<a name="new_MalformedPayloadError"></a>
##new MalformedPayloadError(msg)
Payload is malformed or cannot be parsed.

**Params**

- msg   

<a name="EncodingError"></a>
#class: EncodingError
**Members**

* [class: EncodingError](#EncodingError)
  * [new EncodingError(msg)](#new_EncodingError)

<a name="new_EncodingError"></a>
##new EncodingError(msg)
Given object cannot be encoded successfully.

**Params**

- msg   

<a name="OverCapacityError"></a>
#class: OverCapacityError
**Members**

* [class: OverCapacityError](#OverCapacityError)
  * [new OverCapacityError(msg)](#new_OverCapacityError)

<a name="new_OverCapacityError"></a>
##new OverCapacityError(msg)
Violation of AMQP flow control.

**Params**

- msg   

<a name="AuthenticationError"></a>
#class: AuthenticationError
**Members**

* [class: AuthenticationError](#AuthenticationError)
  * [new AuthenticationError(msg)](#new_AuthenticationError)

<a name="new_AuthenticationError"></a>
##new AuthenticationError(msg)
Authentication failure.

**Params**

- msg   

<a name="ArgumentError"></a>
#class: ArgumentError
**Members**

* [class: ArgumentError](#ArgumentError)
  * [new ArgumentError(arg)](#new_ArgumentError)

<a name="new_ArgumentError"></a>
##new ArgumentError(arg)
Argument missing or incorrectly defined.

**Params**

- arg   

<a name="InvalidStateError"></a>
#class: InvalidStateError
**Members**

* [class: InvalidStateError](#InvalidStateError)
  * [new InvalidStateError(msg)](#new_InvalidStateError)

<a name="new_InvalidStateError"></a>
##new InvalidStateError(msg)
Invalid state.

**Params**

- msg   

<a name="AttachFrame"></a>
#class: AttachFrame
**Members**

* [class: AttachFrame](#AttachFrame)
  * [new AttachFrame()](#new_AttachFrame)

<a name="new_AttachFrame"></a>
##new AttachFrame()
<h2>attach performative</h2>

<a name="BeginFrame"></a>
#class: BeginFrame
**Members**

* [class: BeginFrame](#BeginFrame)
  * [new BeginFrame()](#new_BeginFrame)

<a name="new_BeginFrame"></a>
##new BeginFrame()
<h2>begin performative</h2>

<a name="CloseFrame"></a>
#class: CloseFrame
**Members**

* [class: CloseFrame](#CloseFrame)
  * [new CloseFrame()](#new_CloseFrame)

<a name="new_CloseFrame"></a>
##new CloseFrame()
<h2>close performative</h2>

<a name="DetachFrame"></a>
#class: DetachFrame
**Members**

* [class: DetachFrame](#DetachFrame)
  * [new DetachFrame()](#new_DetachFrame)

<a name="new_DetachFrame"></a>
##new DetachFrame()
<h2>detach performative</h2>

<a name="DispositionFrame"></a>
#class: DispositionFrame
**Members**

* [class: DispositionFrame](#DispositionFrame)
  * [new DispositionFrame()](#new_DispositionFrame)

<a name="new_DispositionFrame"></a>
##new DispositionFrame()
<h2>disposition performative</h2>

<a name="EndFrame"></a>
#class: EndFrame
**Members**

* [class: EndFrame](#EndFrame)
  * [new EndFrame()](#new_EndFrame)

<a name="new_EndFrame"></a>
##new EndFrame()
<h2>end performative</h2>

<a name="FlowFrame"></a>
#class: FlowFrame
**Members**

* [class: FlowFrame](#FlowFrame)
  * [new FlowFrame()](#new_FlowFrame)

<a name="new_FlowFrame"></a>
##new FlowFrame()
<h2>flow performative</h2>

<a name="Frame"></a>
#class: Frame
**Members**

* [class: Frame](#Frame)
  * [new Frame()](#new_Frame)
  * [frame.outgoing()](#Frame#outgoing)
  * [frame.readPerformative(describedType)](#Frame#readPerformative)

<a name="new_Frame"></a>
##new Frame()
Encapsulates all convenience methods required for encoding a frame to put it out on the wire, and decoding an
incoming frame.

Frames look like:

 <pre>
             +0       +1       +2       +3
        +-----------------------------------+ -.
      0 |                SIZE               |  |
        +-----------------------------------+  |-- > Frame Header
      4 |  DOFF  |  TYPE  | &lt;TYPE-SPECIFIC&gt; |  |      (8 bytes)
        +-----------------------------------+ -'
        +-----------------------------------+ -.
      8 |                ...                |  |
        .                                   .  |-- > Extended Header
        .          &lt;TYPE-SPECIFIC&gt;          .  |  (DOFF * 4 - 8) bytes
        |                ...                |  |
        +-----------------------------------+ -'
        +-----------------------------------+ -.
 4*DOFF |                                   |  |
        .                                   .  |
        .                                   .  |
        .                                   .  |
        .          &lt;TYPE-SPECIFIC&gt;          .  |-- > Frame Body
        .                                   .  |  (SIZE - DOFF * 4) bytes
        .                                   .  |
        .                                   .  |
        .                           ________|  |
        |                ...       |           |
        +--------------------------+          -'

 </pre>

<a name="Frame#outgoing"></a>
##frame.outgoing()
Populate the internal buffer with contents built based on the options.  SIZE and DOFF will be inferred
based on the options given.

**Access**: private  
<a name="Frame#readPerformative"></a>
##frame.readPerformative(describedType)
Used to populate the frame performative from a DescribedType pulled off the wire.

**Params**

- describedType <code>[DescribedType](#DescribedType)</code> - Details of the frame performative, should populate internal values.  

<a name="AMQPFrame"></a>
#class: AMQPFrame
**Members**

* [class: AMQPFrame](#AMQPFrame)
  * [new AMQPFrame()](#new_AMQPFrame)
  * [aMQPFrame._getPerformative()](#AMQPFrame#_getPerformative)
  * [aMQPFrame._getAdditionalPayload()](#AMQPFrame#_getAdditionalPayload)

<a name="new_AMQPFrame"></a>
##new AMQPFrame()
AMQP Frames are slight variations on the one above, with the first part of the payload taken up
by the AMQP <i>performative</i> (details of the specific frame type).  For some frames, that's the entire payload.

<pre>
      +0       +1       +2       +3
        +-----------------------------------+ -.
      0 |                SIZE               |  |
        +-----------------------------------+  |-- > Frame Header
      4 |  DOFF  |  TYPE  |     CHANNEL     |  |      (8 bytes)
        +-----------------------------------+ -'
        +-----------------------------------+ -.
      8 |                ...                |  |
        .                                   .  |-- > Extended Header
        .             &lt;IGNORED&gt;             .  |  (DOFF * 4 - 8) bytes
        |                ...                |  |
        +-----------------------------------+ -'
        +-----------------------------------+ -.
 4*DOFF |           PERFORMATIVE:           |  |
        .      Open / Begin / Attach        .  |
        .   Flow / Transfer / Disposition   .  |
        .      Detach / End / Close         .  |
        |-----------------------------------|  |
        .                                   .  |-- > Frame Body
        .                                   .  |  (SIZE - DOFF * 4) bytes
        .             PAYLOAD               .  |
        .                                   .  |
        .                           ________|  |
        |                ...       |           |
        +--------------------------+          -'

</pre>

<a name="AMQPFrame#_getPerformative"></a>
##aMQPFrame._getPerformative()
Children should implement this method to translate their internal (friendly) representation into the
representation expected on the wire (a DescribedType(Descriptor, ...) with either a List of values
(ForcedType'd as necessary) or an object containing an encodeOrdering[] array to clarify ordering).

**Access**: private  
<a name="AMQPFrame#_getAdditionalPayload"></a>
##aMQPFrame._getAdditionalPayload()
AMQP Frames consist of two sections of payload - the performative, and the additional actual payload.
Some frames don't have any additional payload, but for those that do, they should override this to generate it.

**Access**: private  
<a name="FrameReader"></a>
#class: FrameReader
**Members**

* [class: FrameReader](#FrameReader)
  * [frameReader.read(cbuf)](#FrameReader#read)
  * [frameReader._readMessage(messageBuf)](#FrameReader#_readMessage)

<a name="FrameReader#read"></a>
##frameReader.read(cbuf)
For now, just process performative headers.

**Params**

- cbuf  - circular buffer containing the potential frame data.  

**Returns**: [AMQPFrame](#AMQPFrame) - Frame with populated data, undefined if frame is incomplete.  Throws exception on unmatched frame.  
<a name="FrameReader#_readMessage"></a>
##frameReader._readMessage(messageBuf)
An AMQP Message is composed of:

* Zero or one header
* Zero or one delivery-annotations
* Zero or one message-annotations
* Zero or one properties
* Zero or one application-properties
* Body: One or more data sections, one or more amqp-sequence sections, or one amqp-value section
* Zero or one footer

**Params**

- messageBuf `Buffer` - Message buffer to decode  

**Returns**: [Message](#Message) - Complete message object decoded from buffer  
**Access**: private  
<a name="OpenFrame"></a>
#class: OpenFrame
**Members**

* [class: OpenFrame](#OpenFrame)
  * [new OpenFrame()](#new_OpenFrame)

<a name="new_OpenFrame"></a>
##new OpenFrame()
<h2>open performative</h2>

<a name="SaslFrame"></a>
#class: SaslFrame
**Members**

* [class: SaslFrame](#SaslFrame)
  * [new SaslFrame()](#new_SaslFrame)

<a name="new_SaslFrame"></a>
##new SaslFrame()
Base Frame for SASL authentication.

To establish a SASL tunnel, each peer MUST start by sending a protocol header. The protocol
header consists of the upper case ASCII letters "AMQP" followed by a protocol id of three,
followed by three unsigned bytes representing the major, minor, and revision of the
specification version (see constants.saslVersion). In total this is an 8-octet sequence:
 <pre>
 4 OCTETS   1 OCTET   1 OCTET   1 OCTET   1 OCTET
 +----------+---------+---------+---------+----------+
 |  "AMQP"  |   %d3   |  major  |  minor  | revision |
 +----------+---------+---------+---------+----------+
 </pre>

Other than using a protocol id of three, the exchange of SASL tunnel headers follows the
same rules specified in the version negotiation section of the transport specification (See
version-negotiation).

The following diagram illustrates the interaction involved in creating a SASL Security Layer:
 <pre>
 TCP Client                 TCP Server
 =========================================
 AMQP%d3.1.0.0  -------- >
 < --------  AMQP%d3.1.0.0
 :
 :
 &lt;SASL negotiation&gt;
 :
 :
 AMQP%d0.1.0.0  -------- >                (over SASL secured connection)
 < --------  AMQP%d0.1.0.0
 open  -------- >
 < --------  open
 </pre>

SASL is negotiated using framing. A SASL frame has a type code of 0x01.
Bytes 6 and 7 of the header are ignored. Implementations SHOULD set these to 0x00. The
extended header is ignored. Implementations SHOULD therefore set DOFF to 0x02.

 <pre>
 type: 0x01 - SASL frame
 +0       +1       +2       +3
 +-----------------------------------+ -.
 0 |                SIZE               |  |
 +-----------------------------------+  |-- > Frame Header
 4 |  DOFF  |  TYPE  |   &lt;IGNORED&gt;&#42;1   |  |      (8 bytes)
 +-----------------------------------+ -'
 +-----------------------------------+ -.
 8 |                ...                |  |
 .                                   .  |-- > Extended Header
 .             &lt;IGNORED&gt;&#42;2           .  |  (DOFF * 4 - 8) bytes
 |                ...                |  |
 +-----------------------------------+ -'
 +-----------------------------------+ -.
 4*DOFF |                                   |  |
 .    Sasl Mechanisms / Sasl Init    .  |
 .   Sasl Challenge / Sasl Response  .  |-- > Frame Body
 .           Sasl Outcome            .  |  (SIZE - DOFF * 4) bytes
 .                           ________|  |
 |                ...       |           |
 +--------------------------+          -'
 &#42;1 SHOULD be set to 0x0000
 &#42;2 Ignored, so DOFF should be set to 0x02
 </pre>

The maximum size of a SASL frame is defined by constants.minMaxFrameSize. There is
no mechanism within the SASL negotiation to negotiate a different size. The frame body of a
SASL frame may contain exactly one AMQP type, whose type encoding must have
sasl-frame. Receipt of an empty frame is an irrecoverable error.

<a name="SaslMechanisms"></a>
#class: SaslMechanisms
**Members**

* [class: SaslMechanisms](#SaslMechanisms)
  * [new SaslMechanisms(options)](#new_SaslMechanisms)

<a name="new_SaslMechanisms"></a>
##new SaslMechanisms(options)
A list of the sasl security mechanisms supported by the sending peer. It is invalid
for this list to be null or empty. If the sending peer does not require its partner
to authenticate with it, then it should send a list of one element with its value as
the SASL mechanism <i>ANONYMOUS</i>. The server mechanisms are ordered in decreasing
level of preference.

**Params**

- options  - Either the DescribedType of an incoming SASL Mechanisms frame,
                 or an array of mechanisms, or a map with a mechanisms key.  

<a name="SaslInit"></a>
#class: SaslInit
**Members**

* [class: SaslInit](#SaslInit)
  * [new SaslInit(options)](#new_SaslInit)

<a name="new_SaslInit"></a>
##new SaslInit(options)
SASL Init frame, containing the following fields:
<table border="1">
    <tr><th>Name</th><th>Type</th><th>Mandatory</th><th>Multiple?</th></tr>
    <tr><td>mechanism</td><td>symbol</td><td>true</td><td>false</td></tr>
    <tr><td>&nbsp;</td><td colspan="3">
The name of the SASL mechanism used for the SASL exchange. If the selected mechanism is
not supported by the receiving peer, it MUST close the Connection with the
authentication-failure close-code. Each peer MUST authenticate using the highest-level
security profile it can handle from the list provided by the partner.
     </td></tr>
     <tr><td>initial-response</td><td>binary</td><td>false</td><td>false</td></tr>
     <tr><td>&nbsp;</td><td colspan="3">
     <i>security response data</i><br/>
     <p>
A block of opaque data passed to the security mechanism. The contents of this data are
defined by the SASL security mechanism.
     </p>
     </td></tr>
     <tr><td>hostname</td><td>string</td><td>false</td><td>false</td></tr>
     <tr><td>&nbsp;</td><td colspan="3">
     <i>the name of the target host</i><br/>
     <p>
The DNS name of the host (either fully qualified or relative) to which the sending peer
is connecting. It is not mandatory to provide the hostname. If no hostname is provided
the receiving peer should select a default based on its own configuration.
     </p>
     <p>
This field can be used by AMQP proxies to determine the correct back-end service to
connect the client to, and to determine the domain to validate the client's credentials
against.
     </p>
     <p>
This field may already have been specified by the server name indication extension as
described in RFC-4366, if a TLS layer is used, in which case this field SHOULD be null
or contain the same value. It is undefined what a different value to those already
specific means.
     </p>
     </td></tr>
</table>

**Params**

- options   

<a name="SaslChallenge"></a>
#class: SaslChallenge
**Members**

* [class: SaslChallenge](#SaslChallenge)
  * [new SaslChallenge(options)](#new_SaslChallenge)

<a name="new_SaslChallenge"></a>
##new SaslChallenge(options)
SASL Challenge frame, containing the following field:

<table border="1">
    <tr><th>Name</th><th>Type</th><th>Mandatory</th><th>Multiple?</th></tr>
    <tr><td>challenge</td><td>binary</td><td>true</td><td>false</td></tr>
    <tr><td>&nbsp;</td><td colspan="3">
Challenge information, a block of opaque binary data passed to the security
mechanism.
    </td></tr>
</table>

**Params**

- options   

<a name="SaslResponse"></a>
#class: SaslResponse
**Members**

* [class: SaslResponse](#SaslResponse)
  * [new SaslResponse(options)](#new_SaslResponse)

<a name="new_SaslResponse"></a>
##new SaslResponse(options)
SASL Response frame, containing the following field:

<table border="1">
    <tr><th>Name</th><th>Type</th><th>Mandatory</th><th>Multiple?</th></tr>
    <tr><td>response</td><td>binary</td><td>true</td><td>false</td></tr>
    <tr><td>&nbsp;</td><td colspan="3">
A block of opaque data passed to the security mechanism. The contents of this data are
defined by the SASL security mechanism.
    </td></tr>
</table>

**Params**

- options   

<a name="SaslOutcome"></a>
#class: SaslOutcome
**Members**

* [class: SaslOutcome](#SaslOutcome)
  * [new SaslOutcome(options)](#new_SaslOutcome)

<a name="new_SaslOutcome"></a>
##new SaslOutcome(options)
This frame indicates the outcome of the SASL dialog. Upon successful completion of the
SASL dialog the Security Layer has been established, and the peers must exchange protocol
headers to either start a nested Security Layer, or to establish the AMQP Connection.

SASL Outcome frame contains the following fields:

<table border="1">
    <tr><th>Name</th><th>Type</th><th>Mandatory</th><th>Multiple?</th></tr>
    <tr><td>code</td><td>sasl-code</td><td>true</td><td>false</td></tr>
    <tr><td>&nbsp;</td><td colspan="3">
    <i>indicates the outcome of the sasl dialog</i><br/>
    </td></tr>
    <tr><td>additional-data</td><td>binary</td><td>false</td><td>false</td></tr>
    <tr><td>&nbsp;</td><td colspan="3">
The additional-data field carries additional data on successful authentication outcome
as specified by the SASL specification (RFC-4422). If the authentication is
unsuccessful, this field is not set.
    </td></tr>
</table>

SASL Code is a ubyte constrained to the following:
<table border="1">
    <tr><th>Byte</th><th>Name</th><th>Details</th></tr>
    <tr><td>0</td><td>ok</td><td>Connection authentication succeeded.</td></tr>
    <tr><td>1</td><td>auth</td><td>
Connection authentication failed due to an unspecified problem with the supplied
credentials.
    </td></tr>
    <tr><td>2</td><td>sys</td><td>
Connection authentication failed due to a system error.
    </td></tr>
    <tr><td>3</td><td>sys-perm</td><td>
Connection authentication failed due to a system error that is unlikely to be corrected
without intervention.
    </td></tr>
    <tr><td>4</td><td>sys-temp</td><td>
Connection authentication failed due to a transient system error.
    </td></tr>
</table>

**Params**

- options   

<a name="TransferFrame"></a>
#class: TransferFrame
**Members**

* [class: TransferFrame](#TransferFrame)
  * [new TransferFrame()](#new_TransferFrame)

<a name="new_TransferFrame"></a>
##new TransferFrame()
<h2>transfer performative</h2>

<a name="PolicyBase"></a>
#class: PolicyBase
**Members**

* [class: PolicyBase](#PolicyBase)
  * [new PolicyBase()](#new_PolicyBase)

<a name="new_PolicyBase"></a>
##new PolicyBase()
Policies encode many of the optional behaviors and settings of AMQP into a cohesive place,
that could potentially be standardized, could be loaded from JSON, etc.

<a name="Sasl"></a>
#class: Sasl
**Members**

* [class: Sasl](#Sasl)
  * [new Sasl()](#new_Sasl)

<a name="new_Sasl"></a>
##new Sasl()
Currently, only supports SASL-PLAIN

<a name="Session"></a>
#class: Session
**Members**

* [class: Session](#Session)
  * [new Session(conn)](#new_Session)
  * [session.sendMessage(link, message, options)](#Session#sendMessage)

<a name="new_Session"></a>
##new Session(conn)
A Session is a bidirectional sequential conversation between two containers that provides a
grouping for related links. Sessions serve as the context for link communication. Any number
of links of any directionality can be <i>attached</i> to a given Session. However, a link
may be attached to at most one Session at a time.

Session states, from AMQP 1.0 spec:

 <dl>
 <dt>UNMAPPED</dt>
 <dd><p>In the UNMAPPED state, the Session endpoint is not mapped to any incoming or outgoing
 channels on the Connection endpoint. In this state an endpoint cannot send or receive
 frames.</p></dd>

 <dt>BEGIN-SENT</dt>
 <dd><p>In the BEGIN-SENT state, the Session endpoint is assigned an outgoing channel number,
 but there is no entry in the incoming channel map. In this state the endpoint may send
 frames but cannot receive them.</p></dd>

 <dt>BEGIN-RCVD</dt>
 <dd><p>In the BEGIN-RCVD state, the Session endpoint has an entry in the incoming channel
 map, but has not yet been assigned an outgoing channel number. The endpoint may receive
 frames, but cannot send them.</p></dd>

 <dt>MAPPED</dt>
 <dd><p>In the MAPPED state, the Session endpoint has both an outgoing channel number and an
 entry in the incoming channel map. The endpoint may both send and receive
 frames.</p></dd>

 <dt>END-SENT</dt>
 <dd><p>In the END-SENT state, the Session endpoint has an entry in the incoming channel map,
 but is no longer assigned an outgoing channel number. The endpoint may receive frames,
 but cannot send them.</p></dd>

 <dt>END-RCVD</dt>
 <dd><p>In the END-RCVD state, the Session endpoint is assigned an outgoing channel number,
 but there is no entry in the incoming channel map. The endpoint may send frames, but
 cannot receive them.</p></dd>

 <dt>DISCARDING</dt>
 <dd><p>The DISCARDING state is a variant of the END-SENT state where the <code>end</code>
 is triggered by an error. In this case any incoming frames on the session MUST be
 silently discarded until the peer's <code>end</code> frame is received.</p></dd>
 </dl>

 <pre>
                         UNMAPPED< ------------------+
                            |                        |
                    +-------+-------+                |
            S:BEGIN |               | R:BEGIN        |
                    |               |                |
                   \\|/             \\|/               |
                BEGIN-SENT      BEGIN-RCVD           |
                    |               |                |
                    |               |                |
            R:BEGIN |               | S:BEGIN        |
                    +-------+-------+                |
                            |                        |
                           \\|/                       |
                          MAPPED                     |
                            |                        |
              +-------------+-------------+          |
 S:END(error) |       S:END |             | R:END    |
              |             |             |          |
             \\|/           \\|/           \\|/         |
          DISCARDING     END-SENT      END-RCVD      |
              |             |             |          |
              |             |             |          |
        R:END |       R:END |             | S:END    |
              +-------------+-------------+          |
                            |                        |
                            |                        |
                            +------------------------+
  </pre>

There is no obligation to retain a Session Endpoint when it is in the UNMAPPED state, i.e.
the UNMAPPED state is equivalent to a NONEXISTENT state.

Note: This implementation *assumes* it is the client, and thus will always be the one BEGIN-ing a Session.

**Params**

- conn <code>[Connection](#Connection)</code> - Connection to bind session to.  

<a name="Session#sendMessage"></a>
##session.sendMessage(link, message, options)
**Params**

- link `Link`  
- message <code>[Message](#Message)</code>  
- options `*`  

<a name="Types"></a>
#class: Types
**Members**

* [class: Types](#Types)
  * [new Types()](#new_Types)
  * [types._listBuilder(val, bufb, codec, [width])](#Types#_listBuilder)
  * [types._arrayBuilder(val, bufb, codec, [width])](#Types#_arrayBuilder)
  * [types._mapBuilder(val, bufb, codec, [width])](#Types#_mapBuilder)
  * [types._initTypesArray()](#Types#_initTypesArray)
  * [types._initEncodersDecoders()](#Types#_initEncodersDecoders)

<a name="new_Types"></a>
##new Types()
Type definitions, encoders, and decoders - used extensively by [Codec](#Codec).

<a name="Types#_listBuilder"></a>
##types._listBuilder(val, bufb, codec, [width])
Encoder for list types, specified in AMQP 1.0 as:
 <pre>
                       +----------= count items =----------+
                       |                                   |
   n OCTETs   n OCTETs |                                   |
 +----------+----------+--------------+------------+-------+
 |   size   |  count   |      ...    /|    item    |\ ...  |
 +----------+----------+------------/ +------------+ \-----+
                                   / /              \ \
                                  / /                \ \
                                 / /                  \ \
                                +-------------+----------+
                                | constructor |   data   |
                                +-------------+----------+

              Subcategory     n
              =================
              0xC             1
              0xD             4
 </pre>

**Params**

- val `Array` - Value to encode.  
- bufb `builder` - Buffer-builder to write encoded list into.  
- codec <code>[Codec](#Codec)</code> - Codec to use for encoding list entries.  
- \[width\] `Number` - Should be 1 or 4.  If given, builder assumes code already written, and will ensure array is encoded to the given byte-width type.  Useful for arrays.  

**Access**: private  
<a name="Types#_arrayBuilder"></a>
##types._arrayBuilder(val, bufb, codec, [width])
All array encodings consist of a size followed by a count followed by an element constructor
 <pre>
                                             +--= count elements =--+
                                             |                      |
   n OCTETs   n OCTETs                       |                      |
 +----------+----------+---------------------+-------+------+-------+
 |   size   |  count   | element-constructor |  ...  | data |  ...  |
 +----------+----------+---------------------+-------+------+-------+

                         Subcategory     n
                         =================
                         0xE             1
                         0xF             4
 </pre>

**Params**

- val <code>[AMQPArray](#AMQPArray)</code> - Value to encode.  
- bufb `builder` - Buffer-builder to encode array into.  
- codec <code>[Codec](#Codec)</code> - Codec to use for encoding array values.  Passed into encoder.  
- \[width\] `Number` - Should be 1 or 4.  If given, builder assumes code already written, and will ensure array is encoded to the given byte-width type.  Useful for arrays.  

**Access**: private  
<a name="Types#_mapBuilder"></a>
##types._mapBuilder(val, bufb, codec, [width])
A map is encoded as a compound value where the constituent elements form alternating key value pairs.
 <pre>
  item 0   item 1      item n-1    item n
 +-------+-------+----+---------+---------+
 | key 1 | val 1 | .. | key n/2 | val n/2 |
 +-------+-------+----+---------+---------+
 </pre>

**Params**

- val `Object` - Value to encode.  
- bufb `builder` - Buffer-builder to encode map into.  
- codec <code>[Codec](#Codec)</code> - Codec to use for encoding keys and values.  
- \[width\] `Number` - Should be 1 or 4.  If given, builder assumes code already written, and will ensure array is encoded to the given byte-width type.  Useful for arrays.  

**Access**: private  
<a name="Types#_initTypesArray"></a>
##types._initTypesArray()
Initialize list of all types.  Each contains a number of encodings, one of which contains an encoder method and all contain decoders.

**Access**: private  
<a name="Types#_initEncodersDecoders"></a>
##types._initEncodersDecoders()
Initialize all encoders and decoders based on type array.

**Access**: private  
<a name="AMQPArray"></a>
#class: AMQPArray
**Members**

* [class: AMQPArray](#AMQPArray)
  * [new AMQPArray(arr, elementType)](#new_AMQPArray)

<a name="new_AMQPArray"></a>
##new AMQPArray(arr, elementType)
Encoding for AMQP Arrays - homogeneous typed collections.  Provides the CODE for the element type.

**Params**

- arr `Array` - Array contents, should be encode-able to the given code type.  
- elementType `Number` - BYTE code-point for the array values (e.g. 0xA1).  

<a name="DescribedType"></a>
#class: DescribedType
**Members**

* [class: DescribedType](#DescribedType)
  * [new DescribedType(descriptor, value)](#new_DescribedType)

<a name="new_DescribedType"></a>
##new DescribedType(descriptor, value)
Described type, as described in the AMQP 1.0 spec as follows:
<pre>
             constructor                       untyped bytes
                  |                                 |
      +-----------+-----------+   +-----------------+-----------------+
      |                       |   |                                   |
 ...  0x00 0xA1 0x03 "URL" 0xA1   0x1E "http://example.org/hello-world"  ...
           |             |  |     |                                   |
           +------+------+  |     |                                   |
                  |         |     |                                   |
             descriptor     |     +------------------+----------------+
                            |                        |
                            |         string value encoded according
                            |             to the str8-utf8 encoding
                            |
                 primitive format code
               for the str8-utf8 encoding

</pre>

**Params**

- descriptor  - Descriptor for the type (can be any valid AMQP type, including another described type).  
- value  - Value of the described type (can also be any valid AMQP type, including another described type).  

<a name="ForcedType"></a>
#class: ForcedType
**Members**

* [class: ForcedType](#ForcedType)
  * [new ForcedType(typeName, value)](#new_ForcedType)

<a name="new_ForcedType"></a>
##new ForcedType(typeName, value)
ForcedType coerces the encoder to encode to the given type, regardless of what it might think.

**Params**

- typeName  - Symbolic name or specific code (e.g. 'long', or 0xA0)  
- value  - Value to encode, should be compatible or bad things will occur  

<a name="Header"></a>
#class: Header
**Members**

* [class: Header](#Header)
  * [new Header(options)](#new_Header)

<a name="new_Header"></a>
##new Header(options)
**Params**

- options   

<a name="DeliveryAnnotations"></a>
#class: DeliveryAnnotations
**Members**

* [class: DeliveryAnnotations](#DeliveryAnnotations)
  * [new DeliveryAnnotations(annotations)](#new_DeliveryAnnotations)

<a name="new_DeliveryAnnotations"></a>
##new DeliveryAnnotations(annotations)
**Params**

- annotations   

<a name="Annotations"></a>
#class: Annotations
**Members**

* [class: Annotations](#Annotations)
  * [new Annotations(annotations)](#new_Annotations)

<a name="new_Annotations"></a>
##new Annotations(annotations)
**Params**

- annotations   

<a name="Properties"></a>
#class: Properties
**Members**

* [class: Properties](#Properties)
  * [new Properties(options)](#new_Properties)

<a name="new_Properties"></a>
##new Properties(options)
**Params**

- options   

<a name="ApplicationProperties"></a>
#class: ApplicationProperties
**Members**

* [class: ApplicationProperties](#ApplicationProperties)
  * [new ApplicationProperties(properties)](#new_ApplicationProperties)

<a name="new_ApplicationProperties"></a>
##new ApplicationProperties(properties)
**Params**

- properties   

<a name="Footer"></a>
#class: Footer
**Members**

* [class: Footer](#Footer)
  * [new Footer(map)](#new_Footer)

<a name="new_Footer"></a>
##new Footer(map)
**Params**

- map   

<a name="Data"></a>
#class: Data
**Members**

* [class: Data](#Data)
  * [new Data(data)](#new_Data)

<a name="new_Data"></a>
##new Data(data)
**Params**

- data   

<a name="AMQPSequence"></a>
#class: AMQPSequence
**Members**

* [class: AMQPSequence](#AMQPSequence)
  * [new AMQPSequence(values)](#new_AMQPSequence)

<a name="new_AMQPSequence"></a>
##new AMQPSequence(values)
**Params**

- values   

<a name="AMQPValue"></a>
#class: AMQPValue
**Members**

* [class: AMQPValue](#AMQPValue)
  * [new AMQPValue(value)](#new_AMQPValue)

<a name="new_AMQPValue"></a>
##new AMQPValue(value)
**Params**

- value   

<a name="Message"></a>
#class: Message
**Members**

* [class: Message](#Message)
  * [new Message(contents, body)](#new_Message)

<a name="new_Message"></a>
##new Message(contents, body)
Actual AMQP Message, which as defined by the spec looks like:
 <pre>
                                                      Bare Message
                                                            |
                                      .---------------------+--------------------.
                                      |                                          |
 +--------+-------------+-------------+------------+--------------+--------------+--------+
 | header | delivery-   | message-    | properties | application- | application- | footer |
 |        | annotations | annotations |            | properties   | data         |        |
 +--------+-------------+-------------+------------+--------------+--------------+--------+
 |                                                                                        |
 '-------------------------------------------+--------------------------------------------'
                                             |
                                      Annotated Message
 </pre>

**Params**

- contents   
- body   

<a name="Symbol"></a>
#class: Symbol
**Members**

* [class: Symbol](#Symbol)
  * [new Symbol(str)](#new_Symbol)

<a name="new_Symbol"></a>
##new Symbol(str)
Encoding for AMQP Symbol type, to differentiate from strings.  More terse than ForcedType.

**Params**

- str `String` - Symbol contents  

<a name="assertArguments"></a>
#assertArguments(options, argnames)
Convenience method to assert that a given options object contains the required arguments.

**Params**

- options   
- argnames   

<a name="encoder"></a>
#encoder(val, buf, [codec])
Encoder methods are used for all examples of that type and are expected to encode to the proper type (e.g. a uint will

**Params**

- val  - Value to encode (for fixed value encoders (e.g. null) this will be ignored)  
- buf `builder` - Buffer-builder into which to write code and encoded value  
- \[codec\] <code>[Codec](#Codec)</code> - If needed, the codec to encode other values (e.g. for lists/arrays)  

<a name="decoder"></a>
#decoder(buf, [codec])
Decoder methods decode an incoming buffer into an appropriate concrete JS entity.

**Params**

- buf `Buffer` - Buffer to decode, stripped of prefix code (e.g. 0xA1 0x03 'foo' would have the 0xA1 stripped)  
- \[codec\] <code>[Codec](#Codec)</code> - If needed, the codec to decode sub-values for composite types.  

**Returns**:  - Decoded value  
<a name="onUndef"></a>
#onUndef(arg1, arg2)
Simple, *light-weight* function for coalescing an argument with a default.

**Params**

- arg1   
- arg2   

**Returns**:  - arg2 if arg1 === undefined, otherwise arg1  
<a name="orDefaults"></a>
#orDefaults(map, defaultMap)
Adds missing values to map from defaultMap.  Mutates input.

**Params**

- map   
- defaultMap   

**Returns**:  - map to allow for chaining.  
<a name="payload"></a>
#payload
Convenience methods for operating against DescribedType list payloads.

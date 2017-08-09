# Base64 for C#
C# �p�� Base64 �G���R�[�_
�׋��p�ɍ�������́D���\�]���Ȃǂ͂��ĂȂ��D

## Encode
### string
�C�ӂ̕����R�[�h���w�肵�ĕ�������G���R�[�h

```csharp
IEnumerable<char> encoded = Base64Encoder.Encode("ABCDEFG", Encoding.ASCII);
```

### bytes
byte[] ���G���R�[�h����ꍇ

```csharp
byte[] source = new byte {0x10, 0x11, 0x12};
IEnumerable<char> encoded = Base64Encoder.Encode(source);
```

## Decode
### string
�C�ӂ̕����R�[�h���w�肵�ăf�R�[�h

```csharp
IEnumerable<char> encoded = // ...
string decoded = Base64Encoder.Decode(encoded, Encoding.ASCII);
```

### bytes

```csharp
IEnumerable<char> encoded = // ...
IEnumerable<byte> decoded = Base64Encoder.Decode(encoded);
```
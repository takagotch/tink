### tink
---
https://github.com/google/tink

```java
import com.google.crypto.tink.config.TinkConfig;
TinkConfig.register();

import com.goolge.crypto.tink.Aead;
import com.google.crypto.tink.KeysetHandle;
import com.google.crypto.tink.aead.AeadKeyTemplates;

KeysetHandle keysetHandle = KeysetHandle.generateNew(
  AeadKeyTemplates.AES128_GCM);
Aead aead = keysetHandle.getPrimitive(Aead.class);
byte[] ciphertext = aead.encrypt(plaintext, associatedData);
```

```
```

```
```

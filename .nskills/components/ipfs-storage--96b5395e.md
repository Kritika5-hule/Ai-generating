# IPFS Storage

| Field | Value |
|-------|-------|
| Type | `ipfs-storage` |
| ID | `96b5395e` |
| Category | app |
| Tags | ipfs, storage, pinata, decentralized, metadata |
| Description | Decentralized storage (Pinata/Web3.Storage) |

## Configuration

| Setting | Value |
|---------|-------|
| Provider | pinata |
| Generate Metadata Schemas | Enabled |
| Generate U I | Enabled |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `PINATA_API_KEY` | Pinata API key | Yes | Yes |  |
| `PINATA_SECRET_KEY` | Pinata secret API key | Yes | Yes |  |
| `NEXT_PUBLIC_PINATA_GATEWAY` | Pinata gateway URL | No | No | https://gateway.pinata.cloud |

## Documentation

### IPFS Storage

# IPFS Storage

Decentralized file storage using Pinata.

## Usage

```typescript
import { useIPFS } from '@/hooks/useIPFS';

function UploadForm() {
  const { upload, isUploading } = useIPFS();
  
  const handleUpload = async (file: File) => {
    const { cid, url } = await upload(file);
    console.log('Uploaded:', url);
  };
}
```


## File Structure

This component would generate the following files:

- `storage-client.ts` (frontend-lib)
- `useIPFS.ts` (frontend-hooks)
- `FileUpload.tsx` (frontend-components)

## Integration Points

**Depends on:**
- Erc721-stylus (`34aead19`)


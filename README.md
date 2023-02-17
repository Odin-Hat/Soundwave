# SoundWave

<p>SoundWave é um bot de música para o discord.</p>
<p>Use como desejar esse bot. Mas devo lembrar que esse é um modelo que você pode usar.</p>
<p>Ele usa as bibliotecas `discord.py`, `asyncio`, `youtube_dl` então certifique-se de ter baixado corretamente essas dependências</p>

## Funções embutidas:
```
{prefixo}play {link da música}

{prefixo}skip

{prefixo}stop
```

### Você deve mudar o que?
```
TOKEN = 'your_token_here'
PREFIX = '!'
client = commands.Bot(command_prefix=PREFIX)
```

<p>Você deve colocar seu Token na variável `TOKEN`.</p>
<p>Na variável `PREFIX` você deve colocar o que melhor te atende.</p>
> **OBS.: ** O prefixo é aquilo que você vai usar antes do comando.

#### Exemplo de uso:
```
TOKEN = 'your_token_here'
PREFIX = '/'
client = commands.Bot(command_prefix=PREFIX)
```

```
$ /play https://youtu.be/E6QNc0932qs
Soundwave: Música adicionada!
$ /play https://youtu.be/Zi5H7UwZrGg
Soundwave: Música adicionada!
$ /play https://youtu.be/S66soxzoXRc
Soundwave: Música adicionada!
$ /Skip
Soundwave: Próxima música!
$ /stop
Soundwave: Cabô a música!
```

#### O que faz cada comando:
<h3>{prefixo}play {link da música}</h3>
<p>Usando seu prefixo e o comando `PLAY` com o link da música que você quer ele toca a sua música.</p>
<br/>
<h3>{prefixo}skip</h3>
<p>Usando seu prefixo e o comando `SKIP` ele para de tocar a música atual (se tiver música tocando) e passa para a próxima música (se você tiver músicas na sua fila de reprodução)</p>
<h3>{prefixo}stop</h3>
<p>Usando seu prefixo e o comando `STOP` ele para a música</p>

> **OBS.: ** Você pode ver no código que tem um comando chamado `PLAY_SONG` que é um comando básico porque ele passa para outra música assim que termina a atual (se você tiver uma fila de reprodução)

## Criador e Licença:
<p>Autor: CodeOpen / Odin-Hat</p>
<p>Licença: </p>
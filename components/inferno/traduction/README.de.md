[![banner](https://particles.js.org/images/banner3.png)](https://particles.js.org)

# inferno-particles

[![npm](https://img.shields.io/npm/v/inferno-particles)](https://www.npmjs.com/package/inferno-particles) [![npm](https://img.shields.io/npm/dm/inferno-particles)](https://www.npmjs.com/package/inferno-particles)

Offizieller [tsParticles](https://github.com/matteobruni/tsparticles) Inferno-Komponent

[![Slack](https://particles.js.org/images/slack.png)](https://join.slack.com/t/tsparticles/shared_invite/enQtOTcxNTQxNjQ4NzkxLWE2MTZhZWExMWRmOWI5MTMxNjczOGE1Yjk0MjViYjdkYTUzODM3OTc5MGQ5MjFlODc4MzE0N2Q1OWQxZDc1YzI) [![Discord](https://particles.js.org/images/discord.png)](https://discord.gg/hACwv45Hme) [![Telegram](https://particles.js.org/images/telegram.png)](https://t.me/tsparticles)

[![tsParticles Product Hunt](https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=186113&theme=light)](https://www.producthunt.com/posts/tsparticles?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-tsparticles") <a href="https://www.buymeacoffee.com/matteobruni"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a beer&emoji=🍺&slug=matteobruni&button_colour=5F7FFF&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00"></a>

## Installation

```shell

npm install inferno-particles

```

oder

```shell

yarn add inferno-particles

```

## Bedienungsanleitung

### Code

Beispiel:

```javascript
import Particles from "inferno-particles";

class App extends Component {
    render() {
        return (
            <Particles
                id="tsparticles"
                params={{
                    background: {
                        color: {
                            value: "#0d47a1",
                        },
                    },

                    fpsLimit: 120,

                    interactivity: {
                        events: {
                            onClick: {
                                enable: true,

                                mode: "push",
                            },

                            onHover: {
                                enable: true,

                                mode: "repulse",
                            },

                            resize: true,
                        },

                        modes: {
                            bubble: {
                                distance: 400,

                                duration: 2,

                                opacity: 0.8,

                                size: 40,
                            },

                            push: {
                                quantity: 4,
                            },

                            repulse: {
                                distance: 200,

                                duration: 0.4,
                            },
                        },
                    },

                    particles: {
                        color: {
                            value: "#ffffff",
                        },

                        links: {
                            color: "#ffffff",

                            distance: 150,

                            enable: true,

                            opacity: 0.5,

                            width: 1,
                        },

                        collisions: {
                            enable: true,
                        },

                        move: {
                            direction: "none",

                            enable: true,

                            outMode: "bounce",

                            random: false,

                            speed: 6,

                            straight: false,
                        },

                        number: {
                            density: {
                                enable: true,

                                area: 800,
                            },

                            value: 80,
                        },

                        opacity: {
                            value: 0.5,
                        },

                        shape: {
                            type: "circle",
                        },

                        size: {
                            random: true,

                            value: 5,
                        },
                    },

                    detectRetina: true,
                }}
            />
        );
    }
}
```

### Props

| Prop | Typ | Definition |

| --------------- | ------ |
-------------------------------------------------------------------------------------------------------------------- |

| width | string | Die Breite der canvas. |

| height | string | Die Höhe der canvas. |

| options | object | Die Optionen der Partikelinstanz. |

| style | object | das Design des canvas-Elements |

| className | string | Der Klassenname des canvas-wrappers |

| canvasClassName | string | Der Klassenname des canvas. |

| container | object | Die Instanz des [Partikel-Containers]
(https://particles.js.org/docs/modules/Core_Container.html) |

Finde die Konfiguration der Parameter [hier](https://particles.js.org).

### Errors

Sollten Fehler auftreten: `tsParticles` benutzt TypeScript `3.9.6`. Benutze also mindestens 3.8 für die `import type`
Syntax.

## Demos

Klicke [hier](https://particles.js.org) für die Demo-Webseite.

<https://particles.js.org>

[Hier](https://codepen.io/collection/DPOage) gibt es auch eine CodePen-Sammlung, die aktiv gepflegt und geupdated wird.

<https://codepen.io/collection/DPOage>

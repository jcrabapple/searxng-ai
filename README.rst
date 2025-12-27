.. SPDX-License-Identifier: AGPL-3.0-or-later

.. _metasearch engine: https://en.wikipedia.org/wiki/Metasearch_engine
.. _Installation guide: https://docs.searxng.org/admin/installation.html
.. _Configuration guide: https://docs.searxng.org/admin/settings/index.html
.. _CONTRIBUTING: https://github.com/searxng/searxng/blob/master/CONTRIBUTING.rst
.. _LICENSE: https://github.com/searxng/searxng/blob/master/LICENSE

.. figure:: https://raw.githubusercontent.com/searxng/searxng/master/client/simple/src/brand/searxng.svg
   :target: https://searxng.org
   :alt: SearXNG
   :width: 512px


SearXNG is a `metasearch engine`_. Users are neither tracked nor profiled.

✨ Enhanced Features
===================

This fork includes the **Quick Summary** feature - AI-powered intelligent summaries of your search results!

**Quick Summary** leverages OpenAI-compatible APIs to generate concise, relevant summaries from your top search results, helping you find information faster without compromising privacy.

Customize the summary prompt in `quick_summary.py`.

Key enhancements:

- 🤖 **AI-Powered Summaries**: Get instant summaries of search results
- ⚙️ **Configurable**: Choose your preferred AI provider and model
- 🔒 **Privacy-Focused**: Summaries are generated on-demand, your searches remain private
- 🎨 **Seamless Integration**: Clean UI that fits naturally into the SearXNG experience
- 🔧 **User Control**: Enable/disable through preferences

Privacy-Respecting LLM Options
-------------------------------

For maximum privacy, we recommend using **Trusted Execution Environment (TEE)** models or self-hosted solutions:

**TEE-Based Providers (Recommended for Privacy)**

- **Dstack.ai** - TEE-secured inference with verifiable privacy guarantees
- **Phala Network** - Confidential AI powered by TEE technology
- **Secret Network** - Privacy-first blockchain-based AI inference
- **Oasis Network** - Confidential computing for AI workloads

These providers use hardware-based TEEs (like Intel SGX or AMD SEV) to ensure your data is encrypted even during processing, with cryptographic proof that your queries are never logged or accessed.

**Self-Hosted Options**

- **Ollama** (https://ollama.ai) - Run models locally (Llama, Mistral, etc.)
- **LocalAI** (https://localai.io) - OpenAI-compatible API for local models
- **LM Studio** - Desktop app for running LLMs locally
- **vLLM** - High-performance local inference server

**Privacy-Focused Cloud Providers**

- **Mistral AI** - European provider with strong privacy commitments
- **Anthropic (Claude)** - Does not train on user data
- **Together.ai** - Open models with privacy options

**Configuration Example**

To use a TEE or local provider, configure in your preferences::

    Quick Summary Settings:
    - Enable Quick Summary: Yes
    - API Base URL: https://your-tee-provider.com/v1 (or http://localhost:11434/v1 for Ollama)
    - API Key: your-key (not needed for local models)
    - Model: llama3.2 (or your preferred model)

For complete privacy, self-hosted solutions ensure your search queries never leave your infrastructure.

.. image:: https://img.shields.io/badge/organization-3050ff?style=flat-square&logo=searxng&logoColor=fff&cacheSeconds=86400
   :target: https://github.com/searxng
   :alt: Organization

.. image:: https://img.shields.io/badge/documentation-3050ff?style=flat-square&logo=readthedocs&logoColor=fff&cacheSeconds=86400
   :target: https://docs.searxng.org
   :alt: Documentation

.. image:: https://img.shields.io/github/license/searxng/searxng?style=flat-square&label=license&color=3050ff&cacheSeconds=86400
   :target: https://github.com/searxng/searxng/blob/master/LICENSE
   :alt: License

.. image:: https://img.shields.io/github/commit-activity/y/searxng/searxng/master?style=flat-square&label=commits&color=3050ff&cacheSeconds=3600
   :target: https://github.com/searxng/searxng/commits/master/
   :alt: Commits

.. image:: https://img.shields.io/weblate/progress/searxng?server=https%3A%2F%2Ftranslate.codeberg.org&style=flat-square&label=translated&color=3050ff&cacheSeconds=86400
   :target: https://translate.codeberg.org/projects/searxng/
   :alt: Translated

Setup
=====

To install SearXNG, see `Installation guide`_.

To fine-tune SearXNG, see `Configuration guide`_.

Further information on *how-to* can be found `here <https://docs.searxng.org/admin/index.html>`_.

Connect
=======

If you have questions or want to connect with others in the community,
we have two official channels:

- `#searxng:matrix.org <https://matrix.to/#/#searxng:matrix.org>`_
- `#searxng @ libera.chat <https://web.libera.chat/?channel=#searxng>`_ (bridged to Matrix)

Contributing
============

See CONTRIBUTING_ for more details.

License
=======

This project is licensed under the GNU Affero General Public License (AGPL-3.0).
See LICENSE_ for more details.

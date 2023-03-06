# vega-sim-agents
A slimmed-down version of [Vega Market Sim](https://github.com/vegaprotocol/vega-market-sim)'s agents allowing quick inspection and testing.

In order to get set up, install the `requirements.txt` into a python environment of your choice. Directly using `venv` can be a good option for an easy light environment wrapper.

Once installed, the easiest way to start is to run `python -m vega_agents.run_agent`. This will run the simple agent, which doesn't do anything by default, inside a market running from randomly generated prices. To run vs historic prices instead, uncomment the section `price_process_fn` in `run_agent.py`. 

On first run, the code will automatically download the latest version of `vega` core in order to run. This should work on Linux, MacOS and Windows running WSL.

Modify the agent who lives in `vega_agents/agents/simple_agent.py` with the snippets at the top of the file (or anything else) to do some trading.

The `learning_agent` stack can also be run or just inspected for a simple RL loop.

For a much fuller capability set, and instructions on how to get the web console set up to better debug your creations, refer to the full [Vega Market Sim](https://github.com/vegaprotocol/vega-market-sim) repository.

If using the full Vega Market Sim, the same files as are contained within this repository live in `vega_sim.reinforcement` including the simplified agent.

# deploy-rehearsal

A scenario repository of the Kanon e2e harness: the deploy lane's rehearsal (Kanon plan 0012
step E5), at Kanon `candidate-v0.44.0`, in `kanon-e2e/e2e-deploy-rehearsal-42205052362-1`. The harness made it, runs three releases
through Kanon's deploy lane here, and deletes it. Nothing here deploys anywhere: the hooks under
`.github/actions/` build one file, check it arrived, and touch no cloud.

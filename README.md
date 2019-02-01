# Social-context-based-agent-Vehicle-trajectory-prediction
An RNN graphical model architecture

The aim of this project is to develop an agent based
tracking and prediction model for subsequent use in autonomous vehicles. The moving agent tries to learn the
motion behavior of external disturbances and predict their
trajectory and then plan its own path accordingly to avoid
them. We analyze how the human behaves in external circumstances and make the agent learn to mimic these behaviors in given social context. We look at different RNN models such as Vanilla RNN, and then proceed with improved
prediction models such as LSTM and subsequently will use
social grid based agent LSTM model for path planning of
the agent with disturbance behavior as the variables. Stanford drone dataset is used for mapping and training the disturbance motion behavior. The developed model firstly runs
on the test dataset given and generates the predicted trajectory. The social context tensor is used by the agent lstm
with velocity and position vector of the agent, to generate
the agent path.

 The proposed network architecture has a Coordinate Tensor which is based on the coordinates at the given time and a Social Context tensor which is shared with the agent network. This tensor is an embedding which follows the Social Attention LSTM model of social grids. We want our model to learn the essence of relative distances for which gradients are representative of velocity (pool layer).  The concatenation helps the agent LSTM network to learn as much detailed inputs. The final prediction tensor consists sequence of position data of both the disturbances and the agents. 

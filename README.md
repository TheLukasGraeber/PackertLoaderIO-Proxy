        final PacketLoaderIO packetLoaderIO = new PacketLoaderIO("IP", "TOKEN");
        packetLoaderIO.connectMainServers();
        packetLoaderIO.getBungeeCordToSpigotPacket().registerPacket("PACKET", "PACKET");
        if (packetLoaderIO.getBungeeCordToSpigotPacket().isMainPacketRegistered("PACKET")) {
            if (packetLoaderIO.getBungeeCordToSpigotPacket().getPacket("PACKET", 1).equalsIgnoreCase("PACKET")) {
                //Was soll es machen, wenn es positiv ischt?
                packetLoaderIO.getBungeeCordToSpigotPacket().deleteMainPacket("PACKET");
            } else {
                //Was soll es machen, wenn es negative ischt?
            }
        }
